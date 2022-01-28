#### Article 301 · January 12, 2021

### On Machine Learning

# Three Modes of ML Pipelines

### And How to improve the performance of ML Pipelines

"What does an ML Training Pipeline look like?"

In theory, in its simplest form, you train a model based on some data. In practice, all but the most trivial ML systems include a few more steps:

* The raw data might need some preprocessing, and before you do that, you might need to inspect the data.

* You might have to choose what Model to use and set the various hyperparameters of the Model.

* After training the Model, you would want to evaluate it and inspect the results. Any learnings from this inspection process might influence the previous two steps.

* You iterate, until the model is satisfactory.

![Image](https://cdn-images-1.medium.com/max/800/1*aX4gUw685lK2OA7j4x9LFA.png)

While even this more elaborate pipeline is somewhat simplistic, it is sufficient to explore my next question, namely, "How might we improve the performance of this ML Pipeline?"

Broadly, there are three ways:

* Better Data. ML consists of "learning" patterns in past data and using this knowledge to make decisions about the future. For example, learning how to give better product recommendations to a customer on an e-commerce site, based on that customer's and other customers' past behaviour. Better past data, usually helps you make better decisions about the future.

* Better People. Several steps (inspecting data, model choice, inspecting results) benefit from human intelligence, knowledge and experience. Hence, the more intelligent, knowledgeable, and experienced people you have working on your ML systems, the better results you will get.

* Better Process. While a pipeline might feel "linear" our ML Training Pipeline contains a feedback loop. Once you train a model, you evaluate it, inspect the results and iterate; until you have a good enough Model. The better you do this, the getter your models will be, and, hence, the better the performance of your ML Pipeline. In the case of this process, "better" mostly means one thing: "faster". ML is a "search" for the best Model. And the fast you can iterate, the faster you do this search; and the quicker you'll reach a better model.

Which brings us to my third question: "How might we iterate faster?" This question finally brings us to our title topic: "Three Modes of ML Training".

The "Three Modes" are three contrasting yet complementary ways to run the ML pipeline. When used together, they enable fast iteration, and as a result, more performant ML Pipelines.

## Test Mode

What are good qualities would you expect from Unit Tests?

Firstly, you'd want them to execute quickly (i.e. in a few seconds). If it took several hours for your tests to run, you'd probably give up and do something else. Secondly, you'd want them to execute "seamlessly"; for example, it would be convenient if the tests ran automatically each time you made a change or a commit; without you having to run the tests manually.

What have Unit Tests got to do with ML Pipelines?

A significant proportion of ML consists of basic software engineering. Many ML practitioners, especially those who consider ML somehow more superior to "plain programming" don't want to admit this, but this is, nonetheless, true. You can't build efficient ML systems if you aren't a good software engineer (SWE). A good SWE is not just someone who writes good code, but also someone who follows other best practices like Testing.

Sadly, while Testing is vital for ML Pipelines, it is often completely ignored. The only Testing is "testing in production". You know there is someone wrong with your ML Pipeline when it crashes.

ML Training in Test Mode consists of the following: You run every step of the ML pipeline as if it were a test. "As if it were a test" means the following:

* Since tests should execute quickly, you modify any steps that take a lot of time. The most obvious source of slowness in an ML pipeline is the size of data. There is no way you can execute the pipeline in seconds if you need to crunch Terabytes of data. Hence, in Test Mode, you test the pipeline on a small amount of data, say a few thousand rows.

* You will have all the "hooks" in place to ensure that the pipeline runs in Test Mode each to a significant change is made.

* You don't expect the results of Test Mode to be of high quality. For example, a Model trained in Test Mode would not be perfect. However, you won't expect it to be complete garbage either. Hence, you can write UnitTests to validate the pipeline's various steps (like the Model produced).

## Human Mode

As we saw earlier, there are several steps in the ML Pipeline that depend on human intelligence. Human Mode makes it as easy as possible for the humans in the loop to be as intelligent as possible. Let's look at each of the human steps in more detail.

* Inspecting Data. In most ML systems, raw data is stored in vast data lakes, often on specialized servers in the cloud. While these are optimized for storage and processing, they are not optimized for humans. It is not easy for a human to get an intuition for the data on these specialized data sources. When I want to get a "feel" of the data, I download a few thousand rows of data to my local machine and use a combination of standard tools (e.g. Excel) and custom scripts to slice and dice the data. If the data involves images, video, audio and media, I will build a basic dashboard for inspecting the data.

* Model Choices. When you first tackle an ML problem, you usually don't know what algorithm is best. For example, you might want to choose between Boosting and a Neural Net. Even for a single type of algorithm (say a Neural Net), you might not know what Hyper-Parameters (e.g. The number of layers) are optimal. Human mode should make it easy to A) try out, and B) validate many choices quickly. "A)" is enabled by different algorithms having a common interface. "B)", similar to Test Mode, is enabled by training and validating models on a smaller set of local data. You could afford a little more time for the models to train than in TestMode; but you can't afford hours, as the humans involved would get bored. Hence, like the data inspection step, you'd want your data to live locally, or in someplace where access is fast.

* Inspecting Results. In many ways, this is similar to Inspecting Data. You want the humans in the loop for getting a sense of how the models are doing. This involves looking at the data in more detail than a few performance metrics. For example, judging a model on False Positive/Negative Rates or a Confusion Matrix might be insufficient. Instead, the human inspector would want to see what types of features led to False Positives, and what led to Negatives. Like Inspecting Data, this would involve a lot of visualization, custom dashboards and slicing/dicing at will.

There are more and more automated Test Mode tools, but few effective tools for Human Mode; probably because each human and ML problem is different. Humans need to be allowed to apply creativity and adapt. The best ML organizations are those that perfect Human Mode.

## Production Mode

Production Mode is the final Model in the ML Pipeline. By this time, almost all the productive work is complete. Test Mode ensures that the code and other steps work properly. Human Mode ensures that humans have applied their human intelligence and expertise to solve the problem. All that remains is to train the final production model. This almost always involves running the entire pipelines just once, without iteration. These steps rarely need to repeat, or we need to go back to the Human or Test Mode, usually when some specific data breaks the pipeline.

Sadly, many ML pipelines operate only in Production Mode. "Testing in Production" slows down development significantly, and the lack of Human Mode means that models are hardly optimal.

## Some Concluding Thoughts

Having different modes requires some initial investment and thought, but is well worth it — the gains in speed more than make up for the initial cost. Also, many of the principles behind these "modes" make future development more efficient. For example, adhering to "common interface" described in Human Mode make it easy to apply the same pipeline to new problems. Contrastingly, when the only mode available is Production Mode, pipelines need to be rebuilt for every problem.

The organizations that have perfected the "Art of the ML Pipeline", have completely Automated Test Mode and Production Mode. Hence, humans only need to focus on Human Mode; which makes sense because that is the step that depends on Human Intelligence. They also tend to attract the best human ML experts because such experts have the opportunity to exercise their expertise and creativity. In contrast, organizations stuck in Production Mode force their humans to be machines, and waste time drudging in mundane tasks.