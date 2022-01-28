#### Article 293 · November 23, 2020

# Three Stories about QA

### On Software Quality Assurance

## I

"Oh, we don't have to do any testing", replied the developer, almost smugly.

"QA does all our testing", his PM added helpfully. "Our rockstar developers just need to write code fast."

"Who designs the test plan for QA", I ask.

"I do", says the PM.

"Can't the developers write the test plan?" I ask.

"No", says the PM. "Tests plans have a lot of business logic and customer requirements. We don't bother developers with too many details."

"But isn't code full of business logic and customer requirements?", I ask.

"Yes", says the PM hesitantly. "But we spec-it-out so that developers can code it up easily."

I ask to see a test plan, and the PM shares a Word document with about 500 manual test workflows. I show a few workflows to the developer.

"Which part of the code are these tests testing?", I ask the developer.

"That's the Seller page. These code modules and functions."

"Can you open the seller page and test this workflow?"

I expected the developer to open the Seller page on his web-browser. Instead, he opens a terminal and runs a script. Before our eyes, and as if by magic, the script automatically tests the workflow.

"Why did you write the script?" I ask the developer.

"Oh, it makes it easy to test bugs", he replies.

"So you do write tests?", I ask.

"I don't have scripts for all the code", he replies. "Just a few."

"Would it be easy to write automatic tests for all your code?" I ask.

"In theory, yes", he replies.

"But not in practice?" I ask.

"No. That's QA's job".

"But what if you did write more of these test scripts?", I persist.

"Well, reflected the developer. "My code would be much cleaner. And we won't need to spend so much time back-and-forth with QA".

"But your PM would still have to write the plans, right?", I ask.

"Not really. If you understand the business logic well enough to write code, you can also write tests".

## II

"Why do QA engineers get paid less than Developers?" I ask. "After all, don't you all have the same university qualifications? Like degrees in Computer Science?"

"Actually", replied the senior QA engineer, "The pay here is quite good for QAs. We get paid a lot more than other companies."

"Why do you get paid more?" I ask.

"The hours can be tough", she replies. "Particularly during releases and deadlines. Sometimes we are up all night testing."

"Also", she adds doubtfully, "The work can be quite boring."

"Why", I ask.

"Running test after test after test. Manually" she explains. "It can be a pain".

"Could you do it differently?" I ask.

"Well", she replied, "there are a lot of bugs that are not in the test plan."

"How do you know?" I ask.

"Well, when you use the product for a long time like we do, you get a sense of where things might be wrong", says she.

"Do you report these to the PMs and developers?" I ask.

"Sometimes", she replies. "Though usually, we are so busy testing the test plan, there is no time".

"What if you had more time?"

"Yes — we'd test outside the test plan. It is more interesting and creative, and also more useful. Test plans are repetitive. Stupid actually."

"But why don't you have more time?" I ask.

"We don't have a lot of budget for QA. So we only budget for the time needed to finish the test plans."

"Why did you decide to become a QA?", I ask.

"Well — I interviewed for both QA and Developer roles. The interviewer said I'd be better for QA, so I become a QA."

"Ah ok. You probably messed-up the coding question?", I queried.

"There was no coding question. The PM and the CEO said they needed QA people, and I'd be good for the job."

## III

"When we were small, we didn't have a QA team. We shipped a lot of bugs, but since we didn't too many customers, it wasn't a big deal.

"Then we got bigger, and things changed. High-value customers expect more, especially from an enterprise product. Every enterprise product has QA, so we decided to build a QA team. As a sort of extra defensive layer".

"So, what does this defensive layer, defend you against?", I ask the CEO.

"Bugs, of course", he replies.

"Since developers write the bugs, QA defends the company against bad developers, right?"

"Sort of", replies the CEO doubtfully.

"I was looking at one of your manual test plans", I continue. "It looks automated tests can replace most of the manual tests."

"So, you want us to hire you to write the automated tests?", the CEO grins.

"Hardly", I reply

"Then who?", the CEO asks. "You know these consulting companies that design test plans are really expensive. We don't have that kind of money."

"Your own developers care perfectly, capable of writing automated test plans."

"Are they capable?" he asks.

"You don't think so?" I reply

"Well, won't the test plans have a lot of business logic and customer requirements?", he asks.

"Did you look at your test plans?" I ask.

"No — I leave that to my PMs", he replies.

"No", I reply. "‘business logic' and ‘customer requirements', as you put it, won't be a problem to your developers. The can write the automated tests."

"But then what happens to the QA team?, the CEO asks. "What do we do with them?"

"Well, some of them might be excellent developers", I reply.

"And we get rid of the others?", the CEO replies.

"No", I answer. "You're QA team could stay as it is, just fine. Maybe even grow a bit bigger".

"But", the CEO looks at me confused. "What would they do?"

"Well", I say, "They could do what you wanted them to do in the first place. Be your defensive layer."

"But what would they do? If the developers are already writing all the tests?" he asks.

"They could do their own testing. And also check on whether the developers are doing their job."

"But who will tell them what to test?"

"No one. QA already knows what to do. They can understand the code and read the manuals and figure things out."

"But will they catch new bugs?"

"Oh, yes. QA will catch stuff your PM never thought to put in his Test Plan."

"Interesting", replies the CEO, beginning to see some light.

"And they don't need to test only during product launch deadlines. QA can investigate the product all the time. And during normal hours. Without having to stay up all night when something is about to launch."

"And can we pay them less?", the CEO asks.

"You should pay them more.", I reply. "That is if you want this defensive layer to work."

"It is not working now", the CEO muses. For the first time, philosophically.

## Concluding Morals

* Automated QA: Much of what QA does now can and must be automated. Developers should be responsible for this.

* Creative QA: QA can move away from mechanical and boring QA (which automated tests can replace), to creative and interesting QA. QA will transform into a task that requires human intelligence, as opposed to brute-force labour.

* Asynchronous QA: In the old world, QA is the last link in the feature development chain. As a result, products can't ship without hectic, last-minute testing by QA. In the new world with Automated and Creative QA, QA can be parallel and asynchronous to development.

![Image](https://cdn-images-1.medium.com/max/800/1*RaB_WCXV3fOUMRpAqKri7g.jpeg)