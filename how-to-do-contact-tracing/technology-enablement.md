---
description: 'Under construction! :)'
---

# Technology enablement

Technology cannot remove the need for scaled-up workforces to execute contact tracing. However, technology will enable contact tracing workforces to effectively address the unprecedented scale, speed, and accuracy demanded by the COVID-19 crisis. Cloud-based technology tools can accelerate key functions including:

* Workforce management
* Case management
* Alerts
* Call center and triage

Most government organizations already have contact tracing infrastructure and technology support in place for infectious diseases like HIV or syphilis, but this technology may not be easy to adapt to contact tracing for COVID-19. A good first step is to review your existing workflow and infrastructure to identify where you might need to invest in new technologies (versus where your current solution will be sufficient).

Chances are, your underlying technology infrastructure has not been heavily invested in. It probably involves a great deal of manual data entry, manual importing and exporting of files between systems, paper records, software that doesn’t have the right data structure, and one or two people in the IT department or at an external vendor who understand the software or can make changes to it. Your team has found a way to make it work, and come up with their own creative ways to work within the constraints they have been given. Your contact tracing-related databases, if you have electronic databases, can probably only be accessed on old Windows machines in-person at the health department by health department personnel.

Your underlying technology and processes for STD or tuberculosis contact tracing already have found a way to:
* Get information about positive test results from labs to the health department
* Clean or correct the information from labs when there is an error
* View or find contact information for the positive case
* Get in touch with the positive patient and find to inform them of their diagnosis, connect them to care, and interview them about their contacts (this is not always done by the same person or at the same time)
* Interview the positive patient about their contacts (that they might have exposed or might have exposed them), and prioritize based on likelihood of transmission
* Decide which contacts will be notified by the positive patient vs the health department (“provider referral” vs “patient referral”)
* For contacts that will be notified via patient referral, equip the patient with information and possibly referral cards
* Decide whether to give the patient medication to bring their contacts (“expedited partner therapy”), and if so provide them with the necessary medication and instructions
* Find contact information for the positive patient’s contacts who will be notified by the health department
* Get in touch with the contact and find a time to talk to them
* Inform the contact of their possible exposure, and connect them to testing & care as appropriate
* Sometimes, follow up with contact to see whether they were tested
* Train contact tracers on how to perform contact tracing effectively and ensure the privacy of patients and contacts

Technology can play a role in all of these steps, and might already be used by your health department to supplement manual efforts. Chances are though that your underlying technology and processes are not meant to work rapidly for a new disease, much less at the speed and scale needed for comprehensive COVID-19 contact tracing.

### Tech-enabled case identification, management, & prioritization ###

Technology can play a vital role in getting data about cases from labs to the health department. As there become more and more locations that offer COVID-19 testing, this issue of ensuring the quality, speed, and scalability of this process is essential to any contact tracing efforts. Every day of delay between when a patient was symptomatic or tested and when they are interviewed by contact tracers dramatically lessons the impact contact tracing will have.

Your underlying database of positive cases was not built for COVID-19. You might use the state’s system to source new cases, or your county or city might have its own. Test results will come in from hospitals, clinics, private labs, and public labs. These results might come in electronically through an online integration or portal as HL7 feeds, CSVs, or other raw data files. They also might be entered in by hand to the city or state database from someone directly looking up information about the case in the clinic’s EMR \(electronic medical record\) system, by someone who has received a paper copy of the lab, or by a courier who has brought an electronic file to the city, county, or state on a thumb drive, CD-ROM, or floppy drive. Ideally, you would set up secure electronic integrations between labs and your state, county, and cities so that data can be sent instantly and without alteration.

Even if you are able to get electronic data directly from the lab, the data from the lab will not be free of typos. Patient names and contact information will inevitably be misspelled, because usually this information is hand-written by the patient on a paper form, and then manually typed in by someone at the lab or by the healthcare provider. Anywhere along the chain, technology can play a role in flagging and even automatically correcting common errors, such as “gnail.com” or “gmail.con.” The earlier along the chain this correction happens, the better. Technologies that enable patients to register electronically during or before their visit to the lab, and that conduct field checks on the data entered by the patient \(e.g. a phone number is missing a digit\), will help ensure that the data seen by contact tracers is accurate.

Your system might also need to adapt to treat patients who were never tested or whose test results are pending as presumptive positives in need of care and/or contact tracing. Lab data alone will not then get you the information you need, and further integrations and processes to get data from providers will be necessary.

In addition to getting data from providers and labs, your system will need to know how to interpret those data to flag what cases should be interviewed. A patient could be tested twice with a PCR test on the same day, and have one test come back positive and another negative. A patient could get tested for antibodies and have a positive antibody test, but no longer be worthwhile to interview for contact tracing. Your database and processes will need to handle patients getting tested more than once, with multiple types of tests that mean different things, at many different locations.

Even with a large number of contact tracers, you will need to have the ability to prioritize among positive patients, and your database needs to have the information in it that would guide this prioritization. Examples of data that would be useful \(beyond “test result negative vs positive”\) include:

* Date of test
* Type of test
* Date of symptom onset \(might not be available in lab data, but is helpful for determining infectious period & original date of infection\)
* Other test results for the same patient
* Risk factors \(?\)

Lastly, your contact tracers need to have access to the database of patients they need to interview \(“index cases”\), and know which ones to reach out to. This does not need to be the same database your health department uses because:

* COVID-19 contact tracers only need access to data about a subset of all infectious disease patients, and a subset of COVID-19 cases
* your department database might not be accessible to people who are not in-person using health department desktops
* there might not be an underlying need for your department database to have information about COVID-19 contacts in it

If you do separate your systems, you’ll need to figure out how to get data from your department database of cases into any database / technology being used by contact tracers, and identify which of these databases is the “source of truth” on COVID-19 cases. If it’s your department database, you’ll want to develop a process or integration that allows contact tracers to flag things that are “off” about COVID-19 patient information, such as a disconnected phone number or an email that bounces back, and ensure that information can be corrected in both the database that contact tracers are using and the database being used by the department for the tracking and management of COVID-19 cases.

### Tech-enabled case interviews, contact elicitation, & contact investigation

Once you have your database of cases, cases need to be informed of their diagnosis and interviewed. Quite a bit needs to happen in order to connect the index case to care, ensure they are less likely to infect others \(e.g. connect them to an isolation hotel if they can’t isolate at home\), and elicit contacts. You’ll need to decide who is in charge of what part of this, and whether the person interviewing a patient about their contacts and possible sources of exposure is also performing other functions such as delivering test results or connecting patients to care. If they are performing these other functions, you’ll want to ensure that any database they use allows them to track these activities appropriately.

Technology can play an important role in delivering test results, and even in helping supplement contact elicitation interviews that would otherwise be done on the phone. Some health departments are using third-party vendors like [Healthvana](http://healthvana.com/) to deliver COVID-19 test results and instruct positive patients on which contacts to notify and how to notify them. Index case interviews can be done digitally as well, by having patients fill out an online form about their close contacts and recent activities. These forms are not perfect - not all index cases will feel comfortable filling them out or have private internet access, the form won’t be able to ask probing questions that an interviewer might, and a form can’t build rapport or demonstrate empathy the way a human can. But these forms can scale well, can be available in multiple languages, can be filled out by the patient at any time, and can improve the speed of and accuracy of data collection versus a traditional interview.

Technology can also help with prompting the index patient to remember their contacts or possible exposures. An interviewer can ask an index case to look at their calendar, their text messages, their food delivery apps, their phone geolocation data, and other sources of private electronic tracking and communication that can help the case to remember when their symptoms started, where they’ve been, and who they had in-person contact with.

In addition to trying to elicit the names of contacts, an interviewer will also try to identify ways to reach out to the contact. The index case might have a variety of ways they communicate with or can locate their close contacts, some of which can be used by contact tracers and others that are best suited for conversations just between the patient themselves and their contact. These could include:

* Phone number
* Email address
* Username in various social media platform \(e.g. dating apps, facebook, instagram, etc\)
* Physical address
* Place of work or places commonly visited

Technology can support this by enabling the index case to search through their various contact lists for multiple methods of getting in touch with their close contacts. This could be done by an app the index case would download onto their smartphone, and then setting up integrations with their phone’s contact list, their email client, and their social media apps. The index case could then search for a given contact’s names in all digital locations simultaneously, enabling them to more easily notify those contacts themselves or provide this information to the interviewer.

Once some information about a contact is given to an interviewer, they might want to do their own search for methods of contacting them, especially if the methods provided by the index case don’t seem to be working. This is also true for instances where the lab provides incomplete information about the index case themselves. Technology can make it easier to search multiple databases simultaneously to try to find alternate methods for contacting individuals.

### Tech-enabled contact prioritization & notification

Once contacts have been elicited, they need to be prioritized for follow-up by contact tracers. In traditional contact tracing, often not every case is notified by the health department, or at least not for all infectious diseases. Often the patient themselves is asked to notify their close contacts as well, and provided with help doing so. This is for several reasons:

* Index patients might not want to provide contact tracers with the names of all their close contacts, especially if the contact is undocumented or if one or both parties were not following local ordinances when they were in touch
* Contacts might not answer the phone when called from an unknown number, or open an email from an unknown email address, whereas they would pick up if a friend was calling
* Health departments rarely have the capacity to reach out to all possible contacts, and want to focus their resources on hard-to-reach contacts that can’t be notified by other means

In addition to prioritizing contacts based off of which need to be contacted via provider-referral \(vs peer-to-peer patient referral\), a health department might also want to prioritize contacts who:

* Are especially likely to have been infected by the index case. This would be influenced by:
  * the timing of the interaction - e.g. contacts who were with the index case three days before symptoms appeared would be less likely to be infected than a contact from the day after symptoms appeared
  * the duration of the interaction - e.g. contacts who were with the index case for 3 hours would be more likely to be infected than those who spent two minutes with the patients
  * the location of the interaction - e.g. contacts who were indoors or in a contained environment like a car with the patient would be more likely to be infected than those who were outside in a park \(we think\)
  * whether the index patient was coughing or engaging in behavior that would increase the probability that an infectious dose of the virus would leave their body and enter the other person
* Are especially likely to infect others, if not notified and/or provided with services, for example:
  * Individuals who live in close quarters with other people
  * Individuals who are working essential jobs and leaving their home regularly
* Are especially likely to develop serious illness, if not notified and/or provided with services, for example:
  * Older individuals
  * Individuals with relevant underlying conditions or who are immunocompromised
* Are especially likely to have infected the index case, for example:
  * Close contacts from 2-14 days, especially around 3-6 days, from before the index case started to show symptoms
  * These are generally prioritized less highly for provider-referral notification, because these contacts might already be past their infectious period

Technology can play an important role in sorting through and prioritizing these contacts on these various vectors, enabling health departments to more rapidly prioritize who to notify in what order, and how much effort to expend on contacts who are not easily reached.

In addition to supporting contact prioritization, technology can help with the notification itself. This can be done by providing contact tracers with templates for outreach that they can use for manual emailing or texting of contacts. This can also be done by automatically alerting contacts using pre-set templates \(e.g. the software sends the text message rather than the contact tracer using their own phone\), or with robo-calls to contacts. These interactions can be tracked or automated in a database such as Salesforce, enabling contact tracers to easily see that status of outreach to contacts.

In addition to supporting the sending of a contact notification, technology can help with connecting the contact to testing and / or care. A number of COVID-19 testing location finders exist, such as [Google](https://www.theverge.com/2020/4/17/21225828/google-showing-covid-19-testing-centers-search-results) or [findcovidtesting.com](https://findcovidtesting.com/).

### Tech-enabled contact follow-up

Once a contact has been notified, you may want to follow up with them to ensure they have been tested, encourage them to stay isolated for the 14 days after exposure, and learn more about their symptoms. An increasing number of technologies are being developed to support this, such as [CommCare](https://www.dimagi.com/commcare/) or [Sara Alert](https://saraalert.org/).

### Peer-to-peer contact notification

Technology can enable patients to notifying their own contacts \(if they know their identities\).

Anonymous peer-to-peer mass partner notification systems already exist for STDs \(e.g., [Tell Your Partner](https://tellyourpartner.org/), [Let Them Know](https://letthemknow.org.au/)\), and are beginning to be adapted to support COVID-19 peer-to-peer notification \(e.g., [Tell Your Contacts](https://tellyourcontacts.org/)\).

In addition to helping diagnosed individuals deliver the message, [templates](http://web.archive.org/web/20161222151021/https://www.sotheycanknow.org/inform/text) could make it easier to figure out what to say and [automated suggestions based on timing of test results and symptom onset](http://web.archive.org/web/20160910061632/https://www.sotheycanknow.org/chlamydia#inform_your_partner) could make it easier to decide who to notify. Technology could also enable automated information distribution to contacts about where/whether to get tested, symptom education and monitoring, guidance on isolation/quarantine, and available support and services.

### Tech-enabled recruiting and training of contact tracers

As we consider rapidly scaling up the contact tracing workforce, technology can play a vital role in recruiting, selecting, and training contact tracers.

[GC Talent Reserve](https://talent.canada.ca/en/response) \([open source code](https://github.com/GCTC-NTGC/TalentCloud)\) is one example of how governments can use technology to recruit contact tracers who are already government employees to fill emergency roles.

[Making Contact: A Training for COVID-19 Contact Tracers](https://www.ncsddc.org/resource/making-contact-a-training-for-covid-19-contact-tracers/) is an example of how technology can be used to rapidly train entry-level COVID-19 contact tracers.

### Support people in isolation

### Emerging Bluetooth technology solutions

Apple and Google recently announced a partnership to leverage Bluetooth LE technology to support voluntary proximity tracking. This could theoretically automate portions of contact tracing: once a case is diagnosed, apps could notify others who were in proximity to the diagnosed individual during the infectious period.[\[1\]](./)

For privacy purposes, this technology relies on a “double opt-in”, meaning that both diagnosed and contacts would have to opt in to be traced or notified.

While this technology has potential, it is in its early stages. Based on our review to date, we do not recommend it be a “load-bearing pillar” of contact tracing work for the following reasons:

* **Insufficient coverage.** Since this approach is voluntary, coverage is limited to those who choose to participate. If only 40% participates \(a liberal estimate given [adoption rates in other countries](https://www.reuters.com/article/us-health-coronavirus-apps/bluetooth-phone-apps-for-tracking-covid-19-show-modest-early-results-idUSKCN2232A0)\), it would still only cover 16% of the population.[\[2\]](./) As a result, a manual contact tracing program is still necessary even with relatively broad adoption.
* **Biased coverage.** We should anticipate [lower adoption in vulnerable populations due to language barriers, limited technology access, and more](https://www.pewresearch.org/internet/fact-sheet/mobile/). As a result, over-reliance on this approach could disproportionately divert resources from vulnerable populations.
* **Still under development.** Google and Apple will be launching APIs in May, which will delay the creation of applications. In addition, accurate proximity algorithms are still under development, and issues such as rates of false positives and margins of error are unknown.
* **Outstanding privacy and security questions.** While Google and Apple are pursuing a privacy-centric approach, ensuring privacy in practice is another matter. Privacy experts have expressed concern that location could potentially be inferred from proximity by, for example, hackers or aggressive nation states.

