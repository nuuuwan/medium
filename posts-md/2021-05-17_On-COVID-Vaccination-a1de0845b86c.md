#### Article 324 · May 17, 2021

# On COVID Vaccination

### A Notification System

Over a million Sri Lankans have got at least one dose of some CoViD-19 Vaccine. And plans are afoot to vaccinate many more people.

However, the vaccination drive so far, has been marred by complaints and process inefficiencies. Many people, some of them old and infirm, have had to queue in the sun or rain for hours. Many have been turned away after the ordeal, because the centre ran out of shots. Others have missed the opportunity for vaccination because of miscommunication or confusion.

I have a list of PHI and MOH phone numbers, and I have got into the habit of calling officials in the morning, asking them if there are any vaccination drives in my neighbourhood. When they reply "No", I ask them if there are plans for drives in the next few days. The usual reply is, "We are only notified the night before — so call again tomorrow".

What if there was a better system? For example, what if there was a system that sent me an SMS saying something like this:

>>> Hi Nuwan,

>>> Please report to *CAMPBELL PARK, COLOMBO 8*, at *9 am on Tuesday, May 18th, 2021*, to get your *Sinopharm* COVID Vaccine.

>>> Please bring your National ID Card and medical documents if relevant.

>>> -Thanks!

>>> Public Health Department — Colombo Municipal Council

![Image](https://cdn-images-1.medium.com/max/800/1*jo8FBsiEfcaISN-E-n9fQw.png)

## Can such a system be built, and will it work?

To answer these questions, we need answers for a few "sub-questions".

### Can this system reach all Sri Lankans?

Yes — almost all Sri Lankans have a mobile phone.

### Can we filter people by age?

Yes — all mobile phone numbers (AFAIK) are associated with the National ID Card (NIC) Number of the owner. The first several digits of the NIC represent the year and date of birth, which we can use to filter notification-receivers by age.

### Can we filter by location?

Yes — mobile phone companies have data that can accurately pinpoint the location of a phone. Hence, if the vaccine is administered at Campbell Park, Colombo 8, phones within a (say) 2km radius can be notified.

### Can we specify time windows for vaccinations?

Yes. Again, we can use NIC numbers for that. The last digit of your NIC is a checksum, that is a function of the other numbers, and evenly distributed between 0 and 9. Hence, about 10% of any large-enough population will gave an NIC ending in a particular digit.

Hence, vaccination time windows can be structured by NIC number. For example, NICs ending in 1 and 2 get 9 am, 3 and 4 get 10 am, etc.

### Can health authorities easily communicate their plans with the phone companies?

Yes. For each vaccination location, health authorities need to communicate the following information to the phone companies:

* Vaccination location (e.g. Campbell Park, Colombo 8)

* Vaccination audience approximate radius (e.g. 2km)

* Vaccination time windows (e.g. "NICs ending in 1 and 2 get 9 am, 3 and 4 get 10 am, etc.")

* Vaccination Information (e.g. "Vaccine Name", "bring medical documents" etc.)

This information can be communicated the day before (as local vaccination officials seem to be), and whether there is a change in schedule. For example, if Campbell park is facing delays, they can send an updated SMS asking me to come at 10.30am and not 9am.

## Concluding Question

Sri Lanka is not exactly technologically deficient. We have so many technology companies for whom the above system is peanuts to build. Software Engineers reading this will tell you that this system is probably a day or two of work.

But if this is the case, then why doesn't such a system already exist? I don't have a good answer. Perhaps you do.

Also, if you'd like to collaborate on building such a system, please let me know.