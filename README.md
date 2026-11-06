<!--
author:   ICoBC - International Council on Badges and Credentials
email:    info@icobc.net
version:  1.0.0
language: en
narrator: UK English Female
comment:  A self-paced Knowledge course that explains the personal data inside credentials, the legal basis, minimisation and retention choices for issuing, earner rights and the duties that apply when platforms, third parties and AI services are involved.
@style
:root { --icobc-navy:#02375B; --icobc-orange:#F78222; --icobc-cyan:#5DCAE7; --icobc-lime:#B1CF37; --icobc-mist:#F1F5F8; --icobc-line:#D8E2E9; --icobc-muted:#4F6576; }
body { font-family: "Open Sans", Arial, sans-serif; }
h1, h2, h3, h4 { color: var(--icobc-navy); }
a { color: var(--icobc-navy); }
table th { background: var(--icobc-mist); color: var(--icobc-navy); }
blockquote { border-left: 4px solid var(--icobc-orange); background: var(--icobc-mist); padding: 8px 16px; }
@end
-->

# Data Protection Basics for Credential Issuers

*The personal data inside a credential and the duties that come with it.*

## About this course

This course is part of the ICoBC Credentialing Skills Framework (ICSF), skill SECP "Security, privacy and data protection", level L1 "Contribute", stage K "Knowledge". The VRITE pillar is Trustworthiness. At this level and stage you explain basic data protection duties and privacy risks when issuing or sharing credentials. Knowledge means understanding concepts, rules and the reasons behind them, so that you can explain and recognise them.

**Who it is for**

- L&D and corporate academy leads
- HR and learning technology owners
- Programme and micro-credential leads
- Quality, registry and admissions staff
- Education IT and credential operations
- Professional bodies and sector associations

No prerequisites. You do not need legal training.

**Learning outcomes**

1. Identify personal data in credentials, evidence and platform logs.
2. Explain legal bases, data minimisation and retention for issuing and verification.
3. Describe earner rights and how to handle requests, including deletion and revocation.
4. Recognise when a data protection impact assessment is needed.

**Workload and format**

Self-paced, about 2 hours of notional learning. Five modules, each with explanation, a worked example, a practice activity and a short quiz. Live or workshop elements are described as facilitator notes and are optional.

**Assessment and badge**

A final knowledge check of 10 scenario-based questions. If you pass, you earn the badge "Data Protection Basics for Credential Issuers (Knowledge, L1)", alignment code ICSF-SECP-L1-K. The badge evidence is the passed knowledge check.

| Outcome | Module | How it is assessed |
|---|---|---|
| 1. Identify personal data in credentials, evidence and platform logs | Personal data in credentials | Module 1 quiz; final knowledge check questions 1 and 2 |
| 2. Explain legal bases, data minimisation and retention for issuing and verification | Legal basis and purpose | Module 2 quiz; final knowledge check questions 3 and 4 |
| 2. Explain legal bases, data minimisation and retention for issuing and verification | Minimise what you publish | Module 3 quiz; final knowledge check questions 5 and 6 |
| 3. Describe earner rights and how to handle requests, including deletion and revocation | Earner rights | Module 4 quiz; final knowledge check questions 7 and 8 |
| 4. Recognise when a data protection impact assessment is needed | Third parties, platforms and transfers | Module 5 quiz; final knowledge check questions 9 and 10 |

> This course gives general educational information. It is not legal advice. Your organisation's data protection officer or legal adviser decides how the rules apply to your situation.

> Completing this course shows that you understand the concepts taught here. It does not prove competence in a job role.

<details>
<summary>Facilitator notes</summary>

Optional kick-off (20 minutes, live or online): ask participants to name one credential type their organisation issues and list every place its data is stored. Keep the list visible and return to it at the end of Module 5. Participants can use their own list for the practice activities.

</details>

## Personal data in credentials

### What counts as personal data

Personal data is any information that relates to an identified or identifiable person. In the EU, the General Data Protection Regulation (GDPR) uses this definition. You do not need a name for data to be personal. If someone can be recognised by combining the data with other information, it is personal data.

A digital credential contains more personal data than most issuers expect. Think about three layers:

- **The credential itself.** Earner name, email address or other identifier, the award title, the issue date, the issuer name, a unique credential identifier and sometimes a link to a public page.
- **The evidence.** Assessment results, grades, portfolios, work samples, recordings, assessor comments, reflective statements and identity documents used for verification.
- **The platform logs.** Login times, IP addresses, device information, email delivery records, verification requests and downloads.

All three layers can identify a person. A credential identifier that looks like a random number is still personal data if your system can link it to an earner.

Some data needs extra care. The GDPR sets stricter rules for special categories of data, for example health data. Evidence can contain such data without anyone planning it. A reasonable adjustment record for an exam, a medical note in a portfolio or a photograph of a person in a workshop can bring special category data into your records.

<!-- VERIFY: Confirm with the organisation's legal adviser how special category rules apply to evidence files held by the issuer. -->

### Where the data sits

Mapping where data sits is the first practical step in data protection. Credential data tends to spread:

- the learning management system or student record system
- the credential issuing platform
- the earner's wallet or profile
- email systems, spreadsheets and shared drives
- backups and exports
- third-party tools used for proctoring, video or messaging

A data map does not need to be complex. A simple table with the data item, where it is stored, who can see it and how long it is kept is a good start.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg" font-family="Open Sans, Arial, sans-serif">
  <title>A credential split into public and private fields</title>
  <desc>A central credential card is divided into a public side and a private side. The public side lists the award title, the issuer name and the issue date. The private side lists the earner email address, the assessment evidence and the platform logs.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <rect x="40" y="40" width="720" height="370" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="400" y="80" text-anchor="middle" font-size="20" fill="#02375B" font-weight="bold">One credential, two kinds of field</text>
  <rect x="70" y="110" width="320" height="260" rx="6" fill="#FFFFFF" stroke="#02375B" stroke-width="2"/>
  <rect x="70" y="110" width="320" height="40" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="230" y="137" text-anchor="middle" font-size="16" fill="#02375B" font-weight="bold">Public fields</text>
  <text x="90" y="190" font-size="16" fill="#02375B">Award title</text>
  <text x="90" y="230" font-size="16" fill="#02375B">Issuer name</text>
  <text x="90" y="270" font-size="16" fill="#02375B">Issue date</text>
  <text x="90" y="310" font-size="16" fill="#02375B">Credential identifier</text>
  <text x="90" y="350" font-size="14" fill="#4F6576">Earner chooses whether to show a name</text>
  <rect x="410" y="110" width="320" height="260" rx="6" fill="#FFFFFF" stroke="#02375B" stroke-width="2"/>
  <rect x="410" y="110" width="320" height="40" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="570" y="137" text-anchor="middle" font-size="16" fill="#FFFFFF" font-weight="bold">Private fields</text>
  <text x="430" y="190" font-size="16" fill="#02375B">Earner email address</text>
  <text x="430" y="230" font-size="16" fill="#02375B">Assessment evidence</text>
  <text x="430" y="270" font-size="16" fill="#02375B">Assessor comments</text>
  <text x="430" y="310" font-size="16" fill="#02375B">Platform logs</text>
  <text x="430" y="350" font-size="14" fill="#4F6576">Restricted access, defined retention</text>
</svg>

### Why identification matters first

You cannot protect what you have not found. Every later duty in this course, such as choosing a legal basis, setting retention periods and answering earner requests, starts from knowing what personal data you hold and where.

**Worked example: A college and a corporate academy map their data**

*Context 1: a college.* A college offers a short course in digital skills and issues a micro-credential. The programme lead and the registry officer list the data. The credential holds the earner name, email address, award title and issue date. The evidence folder holds a final project, the assessor's feedback and, for two earners, a note about extra exam time because of a learning difficulty. The issuing platform logs every login and every verification request. The team marks the extra-time notes as sensitive, because they may reveal health information, and moves them out of the evidence folder into the access-controlled student support record.

*Context 2: a corporate academy.* An HR department issues badges for an internal leadership programme. The badge shows the employee name, the programme title and the date. The manager's rating forms and a recorded role-play session are held as evidence. The learning technology owner notes that the role-play recording shows the faces and voices of colleagues who are not earners, so that data concerns more than one person.

**Practice activity: Build a three-column data map**

Take one credential your organisation issues, or one you can imagine. Create a table with three columns: credential, evidence and platform logs. List at least three personal data items in each column. Mark any item that might be special category data. Then add a fourth note: who outside your team can see each item.

<details>
<summary>Facilitator notes</summary>

In a workshop, pairs swap data maps and look for items the other pair missed, for example backups, email attachments and exports. Allow 25 minutes. Collect common blind spots on a flipchart.

</details>

### Check your understanding

**Question 1.** A credential platform records the IP address of every person who verifies a credential. How should the issuer treat this IP address?

[( )] As non-personal data, because it contains no name
[(X)] As personal data, because it can relate to an identifiable person
[( )] As public data, because verification is public
[( )] As evidence data that is exempt from data protection rules

****
An IP address can relate to an identifiable person, especially when combined with other information. A missing name does not remove the data from the scope of data protection rules. Platform logs are one of the three layers to map.
****

**Question 2.** Which item is most likely to be special category data if it is found in an evidence folder?

[( )] The title of the award
[( )] The date of issue
[(X)] A note about an exam adjustment because of a health condition
[( )] The name of the issuing organisation

****
Information about health is a special category of personal data under the GDPR. Exam adjustment notes can reveal health information and need stricter handling than routine credential fields.
****

**Question 3.** Why is a simple data map useful for a credential issuer?

[( )] It replaces the need for any legal basis
[( )] It lets the issuer publish all data safely
[(X)] It shows what personal data is held, where and who can see it, which supports every later duty
[( )] It is only needed for large organisations

****
A data map is the starting point for choosing legal bases, setting retention periods and answering earner requests. Without it, an issuer cannot say what it holds.
****

**Question 4.** A role-play recording used as evidence shows several colleagues. What does this tell the issuer?

[( )] Only the earner is a data subject
[( )] The recording is anonymous because it is internal
[(X)] The recording contains personal data of more than one person
[( )] The recording is not personal data because it is evidence

****
Evidence can show or mention people other than the earner. Their personal data is protected too, and the issuer must consider them when deciding on use, access and retention.
****

## Legal basis and purpose

### Purpose comes first

Under the GDPR, personal data must be collected for specified, explicit and legitimate purposes. You decide the purpose before you collect the data, and you tell people what it is. Later use of the data must fit with that original purpose.

For a credential issuer, typical purposes are:

- assessing whether an earner met the requirements
- issuing and delivering the credential
- allowing others to verify the credential
- keeping a record so that the issuer can confirm an award in the future
- improving the programme through aggregate analysis

Each purpose needs its own thinking. Data collected to issue a credential is not automatically available for marketing.

### The legal bases

The GDPR lists six legal bases for processing personal data. In your own words, they are:

1. **Consent:** the person freely agrees, with a clear and specific choice.
2. **Contract:** processing is needed to perform a contract with the person, or steps before a contract.
3. **Legal obligation:** a law requires the processing.
4. **Vital interests:** processing protects someone's life.
5. **Public task:** processing is needed for a task in the public interest or an official function.
6. **Legitimate interests:** processing serves a real interest of the organisation or a third party, and it does not override the person's rights and freedoms after a balancing test.

You need one valid legal basis for each purpose. You choose it before processing starts and record it. Special category data needs an additional condition on top of the legal basis.

<!-- VERIFY: Check the exact GDPR articles for the legal bases and for special category conditions before citing article numbers in any adaptation of this course. -->

### Applying the bases to credentials

There is no single right answer for all issuers. Here are common patterns, to be confirmed by your data protection officer:

- Assessing and issuing a credential often rests on contract (the learning agreement or enrolment), or on public task for a public institution.
- Keeping a long-term record of awards may rest on legal obligation, public task or legitimate interests, depending on the sector and country.
- Publishing a credential on a public profile page is a different purpose. The earner usually controls this, so consent is a common basis. Consent should be easy to give and easy to withdraw.
- Sending marketing emails to earners is a separate purpose and needs its own basis.

Consent has a weakness in employment. If an employee depends on an employer, consent may not be freely given. HR departments therefore avoid relying on consent when the employee has little real choice.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg" font-family="Open Sans, Arial, sans-serif">
  <title>From purpose to legal basis</title>
  <desc>Three purposes are shown on the left and matched to a legal basis on the right: issuing the credential matched to contract or public task, public display matched to consent, and marketing matched to its own separate basis. A note says each purpose needs its own basis.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <text x="400" y="45" text-anchor="middle" font-size="20" fill="#02375B" font-weight="bold">Each purpose needs its own legal basis</text>
  <text x="170" y="95" text-anchor="middle" font-size="16" fill="#4F6576">Purpose</text>
  <text x="620" y="95" text-anchor="middle" font-size="16" fill="#4F6576">Example legal basis</text>
  <rect x="40" y="115" width="260" height="70" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="170" y="157" text-anchor="middle" font-size="16" fill="#02375B">Issue the credential</text>
  <rect x="40" y="215" width="260" height="70" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="170" y="257" text-anchor="middle" font-size="16" fill="#02375B">Show it on a public page</text>
  <rect x="40" y="315" width="260" height="70" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="170" y="357" text-anchor="middle" font-size="16" fill="#02375B">Send marketing emails</text>
  <line x1="300" y1="150" x2="480" y2="150" stroke="#02375B" stroke-width="2"/>
  <line x1="300" y1="250" x2="480" y2="250" stroke="#02375B" stroke-width="2"/>
  <line x1="300" y1="350" x2="480" y2="350" stroke="#02375B" stroke-width="2"/>
  <rect x="480" y="115" width="280" height="70" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="620" y="157" text-anchor="middle" font-size="16" fill="#02375B">Contract or public task</text>
  <rect x="480" y="215" width="280" height="70" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="620" y="257" text-anchor="middle" font-size="16" fill="#02375B">Consent, easy to withdraw</text>
  <rect x="480" y="315" width="280" height="70" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="620" y="357" text-anchor="middle" font-size="16" fill="#02375B">Its own separate basis</text>
</svg>

### Telling people what you do

Whatever basis you choose, people have the right to be informed. A privacy notice should say who the issuer is, which data is collected, for which purposes, on which legal basis, who receives it, how long it is kept and how to use their rights. Write the notice in plain language and give it before or at the time of collection.

**Worked example: Public display needs a separate decision**

*Context 1: a training provider.* A training provider issues a certificate of completion to every learner. The legal basis for issuing it is the training contract. The provider's platform has a button "Make my credential public". The programme lead decides that publication is a different purpose. The button is off by default, a short explanation sits next to it, and the learner can switch it off again at any time. The provider records consent only for that purpose.

*Context 2: a corporate academy.* An HR department wants to publish employee badges on the company careers page to show how many staff are certified. The HR lead sees that employees may not feel free to say no. The department chooses an aggregate count, with no names, instead of individual display. Individual display stays possible only if an employee chooses it for their own profile.

**Practice activity: Match purposes and bases**

List four purposes for which your organisation, or an imagined issuer, uses credential data. For each, write the legal basis you think fits and one sentence explaining why. Mark the purposes where you are unsure and note who in your organisation would decide.

<details>
<summary>Facilitator notes</summary>

Invite a data protection officer or legal adviser for a 30-minute question session. Ask participants to bring their uncertain purposes from the practice activity. Remind the group that this course explains concepts and does not replace a legal decision.

</details>

### Check your understanding

**Question 1.** A university issues a micro-credential after an enrolled student completes a course. Which statement is most accurate?

[( )] The university needs no legal basis because the student asked for the credential
[(X)] The university needs a legal basis for each purpose, and issuing may rest on the enrolment contract or a public task
[( )] Consent is the only legal basis allowed
[( )] A legal basis is needed only for marketing

****
Every purpose needs a valid legal basis. Issuing an award linked to enrolment often fits contract or public task. Consent is one basis among six and is not always the right one.
****

**Question 2.** An employer wants to publish all employee badges on a public page and relies on employee consent. What is the main concern?

[( )] Badges can never be published
[( )] Consent is not a legal basis
[(X)] Consent may not be freely given when the person depends on the employer
[( )] The page must be password protected

****
In an employment relationship there is a power imbalance. Consent may not be truly free, so HR teams look for other approaches, such as aggregate publication or letting the employee choose on their own profile.
****

**Question 3.** An issuer collected email addresses to deliver credentials. It now wants to send a newsletter. What should it do?

[( )] Send the newsletter, since it already has the email addresses
[( )] Send the newsletter only to earners who passed
[(X)] Treat the newsletter as a separate purpose, check the legal basis and inform people
[( )] Send the newsletter without telling people

****
Later use must fit the original purpose. A newsletter is a different purpose that needs its own legal basis and clear information to the people concerned.
****

**Question 4.** What should a privacy notice for earners include?

[( )] Only the issuer's postal address
[( )] Only a list of the issuer's staff
[(X)] The data collected, the purposes, the legal basis, recipients, retention and how to use their rights
[( )] Only the technical details of the platform

****
The right to be informed covers who you are, what you collect, why, on which basis, who receives it, how long you keep it and how earners can exercise their rights. The notice should be in plain language.
****

## Minimise what you publish

### Data minimisation

Data minimisation is a core GDPR principle. Personal data must be adequate, relevant and limited to what is necessary for the purpose. Ask for each field: do we need this to achieve the purpose? If not, do not collect it or do not show it.

For credentials, minimisation applies in three places:

- **Collection.** Ask earners only for the data you need. A date of birth is not needed to issue a participation badge in most cases.
- **Display.** A public credential page should show what a verifier needs, such as award title, issuer and date. It rarely needs an email address, a full grade report or a home address.
- **Evidence.** Keep evidence only as long and as detailed as needed to justify the award.

### Public, shared and private

It helps to sort every data item into one of three tiers:

- **Public:** anyone with the link can see it.
- **Shared:** shown to a specific verifier, employer or institution that the earner chooses.
- **Private:** stays with the issuer, or with the earner, and is not shown to others.

Verification needs very little. A verifier usually needs to know that the credential is genuine, who issued it, what it says and whether it is still valid. It does not need to see the assessor's comments. Design verification to return the minimum answer. This is also called privacy by design and by default: the safest setting is the default setting.

### Retention and deletion

Personal data must not be kept longer than necessary for the purpose. This is the storage limitation principle. The GDPR does not set a single number of years. You decide a retention period for each type of data, write it down and apply it. Laws on records, accreditation or employment may require a minimum period for some data. Check these with your legal adviser.

A useful way to think about this is a data lifecycle: collect, use, store, share, review and delete. Each stage has a question. What do we collect and why? Who can use it? Where is it stored? With whom do we share it? When do we review it? When and how do we delete it?

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg" font-family="Open Sans, Arial, sans-serif">
  <title>Data lifecycle from issue to deletion</title>
  <desc>Six boxes in a row show the lifecycle of credential data: collect, issue, share and verify, store, review, delete. Arrows connect the boxes from left to right. A note under the row says that each stage has a retention rule.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <text x="400" y="50" text-anchor="middle" font-size="20" fill="#02375B" font-weight="bold">Credential data lifecycle</text>
  <rect x="20" y="150" width="105" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="72" y="196" text-anchor="middle" font-size="15" fill="#02375B">1 Collect</text>
  <rect x="145" y="150" width="105" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="197" y="196" text-anchor="middle" font-size="15" fill="#02375B">2 Issue</text>
  <rect x="270" y="150" width="105" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="322" y="188" text-anchor="middle" font-size="14" fill="#02375B">3 Share and</text>
  <text x="322" y="208" text-anchor="middle" font-size="14" fill="#02375B">verify</text>
  <rect x="395" y="150" width="105" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="447" y="196" text-anchor="middle" font-size="15" fill="#02375B">4 Store</text>
  <rect x="520" y="150" width="105" height="80" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="572" y="196" text-anchor="middle" font-size="15" fill="#02375B">5 Review</text>
  <rect x="645" y="150" width="105" height="80" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="697" y="196" text-anchor="middle" font-size="15" fill="#FFFFFF">6 Delete</text>
  <line x1="125" y1="190" x2="145" y2="190" stroke="#02375B" stroke-width="2"/>
  <line x1="250" y1="190" x2="270" y2="190" stroke="#02375B" stroke-width="2"/>
  <line x1="375" y1="190" x2="395" y2="190" stroke="#02375B" stroke-width="2"/>
  <line x1="500" y1="190" x2="520" y2="190" stroke="#02375B" stroke-width="2"/>
  <line x1="625" y1="190" x2="645" y2="190" stroke="#02375B" stroke-width="2"/>
  <rect x="60" y="290" width="680" height="70" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="400" y="330" text-anchor="middle" font-size="16" fill="#02375B">Every stage has a retention rule: keep only what the purpose needs</text>
</svg>

### Keeping a verifiable record

Credential issuers face a real tension. The earner may want to delete data, but the issuer may need to keep a minimal record that an award was made, so that it can confirm the award later. A good design keeps this record small: earner name or identifier, award, date and status. Detailed evidence can follow a shorter retention period.

Share the retention schedule with earners in your privacy notice, so that nobody is surprised.

**Worked example: Shortening what is shown and kept**

*Context 1: a university.* A university registry issues digital credentials for a postgraduate certificate. The verification page used to show the earner name, programme, grade band and the email address of the programme office. The quality lead reviews the page against the purpose of verification. The grade band and personal contact details are removed from the public view. The registry keeps a minimal award record for the long term. Assessment scripts follow a shorter retention period set out in the retention schedule, and the schedule is published in the privacy notice. The periods themselves are set by the university with its legal adviser.

*Context 2: a corporate academy.* An HR department issues badges for compliance training. Evidence consists of quiz results per employee. The department decides that the result per question is not needed once the badge is issued. It keeps pass or fail, date and badge identifier, and deletes the question-level data after a short period defined with legal advice. When an employee leaves, the badge record follows the HR retention rules for personnel files.

**Practice activity: Sort fields into three tiers**

Take the data items from your Module 1 data map. Sort them into public, shared and private. For each item you place in public or shared, write the purpose it serves. Remove any item for which you cannot name a purpose. Then propose a retention rule for the three most sensitive items, and note who would approve it.

<details>
<summary>Facilitator notes</summary>

Run a "challenge the field" round: one participant proposes a field for the public page, the others ask "which purpose needs it?" until the group agrees to keep or drop it. About 20 minutes. Keep a record of fields that were dropped, to show how much can be removed.

</details>

### Check your understanding

**Question 1.** What does data minimisation mean for a public credential page?

[( )] Show every field to build trust
[( )] Hide the credential completely
[(X)] Show only the data a verifier needs for the purpose of verification
[( )] Show data only in a PDF

****
Data minimisation limits data to what is necessary for the purpose. A verifier needs to confirm that the credential is genuine, who issued it and what it states. Extra fields add risk without adding value.
****

**Question 2.** What does the storage limitation principle require?

[( )] Keeping all data forever in case it is needed
[( )] Deleting all data on the day of issue
[(X)] Keeping personal data no longer than necessary for the purpose, with defined retention periods
[( )] Storing data only on paper

****
Storage limitation means personal data is kept only as long as needed. The issuer sets, documents and applies retention periods, taking into account legal requirements that may require a minimum period.
****

**Question 3.** A registry wants to be able to confirm awards years later, while an earner asks to remove detailed evidence. What is a sensible design?

[( )] Refuse all deletion
[( )] Delete the award record and the evidence together
[(X)] Keep a minimal award record, and apply a shorter retention period to detailed evidence
[( )] Move all evidence to a public page

****
A minimal record such as name or identifier, award, date and status can serve the long-term purpose of confirming an award. Detailed evidence can be kept for a shorter time, unless a legal requirement says otherwise.
****

**Question 4.** What does "privacy by default" mean when setting up a credential platform?

[( )] Every credential is public until the earner hides it
[(X)] The most privacy-protective setting is the default, and the earner can choose to share more
[( )] Privacy settings are hidden from earners
[( )] The platform collects as much data as possible

****
Privacy by default means that, without any action by the earner, only the necessary data is processed and shown. The earner can choose to share more, for example by making a credential public.
****

## Earner rights

### The rights in plain language

The GDPR gives people rights over their personal data. Earners are data subjects. Their main rights, in plain words, are:

- **To be informed** about how their data is used.
- **Of access:** to get a copy of their data and information about how it is processed.
- **To rectification:** to have wrong data corrected.
- **To erasure:** to have data deleted in certain situations. Sometimes called the right to be forgotten.
- **To restrict processing:** to ask you to pause use of their data in certain situations.
- **To data portability:** to receive data they provided in a structured, commonly used format, and to have it passed on, in certain situations.
- **To object:** to object to certain processing, including processing based on legitimate interests or public task.
- **Related to automated decisions:** protections when decisions are made only by automated means with significant effects.

Not every right applies in every case. Which ones apply depends on the legal basis and the situation. The point for an issuer is to recognise a request and send it to the right person quickly.

### Handling a request

Requests do not need a special form. An earner may write an email, use a web form or call. Your staff must be able to recognise a request when it arrives, even if the earner does not use legal words.

A simple process has these steps:

1. **Recognise and log.** Note the date received and who received it.
2. **Verify identity.** Confirm that the person is who they say they are, without asking for more data than needed.
3. **Route.** Send the request to the person responsible, often the data protection officer or privacy contact.
4. **Search.** Check all places on your data map, including platform logs, evidence stores and email.
5. **Decide and respond.** Answer within the legal deadline, explain what you did or why you cannot do it.
6. **Record.** Keep a note of the request and the outcome.

The GDPR sets a general deadline of one month to respond, with a possible extension for complex cases.

<!-- VERIFY: Confirm the response deadline and the conditions for extension in the current GDPR text before publishing. -->

### Deletion and revocation

Two terms are often mixed up, so keep them apart.

- **Revocation** is a credential status action by the issuer. The credential is marked as no longer valid, for example because it was issued by mistake or the earner no longer meets the requirements. Revocation does not necessarily delete personal data. A revocation record may need to be kept so that verifiers can see the status.
- **Deletion** (erasure) is the removal of personal data from your systems. It follows from a request or from the end of a retention period.

An earner may ask for their credential to be deleted. The issuer considers whether the right to erasure applies, whether a legal obligation or other exception means data must be kept, and which part of the data can be removed. Often the answer is partial: the public profile and detailed evidence are removed, and a minimal record is kept where the law or a legitimate purpose requires it. The issuer explains the decision to the earner.

If a credential was shared with others, for example a verifier or a wallet provider, the issuer may need to inform those recipients about deletion or rectification, where this is possible.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg" font-family="Open Sans, Arial, sans-serif">
  <title>Handling an earner request</title>
  <desc>Five steps in a row show how to handle an earner request: recognise and log, verify identity, route, search and decide, respond and record. Below, two separate boxes explain that revocation changes credential status and deletion removes personal data.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <text x="400" y="45" text-anchor="middle" font-size="20" fill="#02375B" font-weight="bold">Handling an earner request</text>
  <rect x="20" y="80" width="135" height="80" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="87" y="125" text-anchor="middle" font-size="15" fill="#FFFFFF">1 Recognise, log</text>
  <rect x="170" y="80" width="135" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="237" y="125" text-anchor="middle" font-size="15" fill="#02375B">2 Verify identity</text>
  <rect x="320" y="80" width="135" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="387" y="125" text-anchor="middle" font-size="15" fill="#02375B">3 Route</text>
  <rect x="470" y="80" width="135" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="537" y="125" text-anchor="middle" font-size="15" fill="#02375B">4 Search, decide</text>
  <rect x="620" y="80" width="160" height="80" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="700" y="125" text-anchor="middle" font-size="15" fill="#02375B">5 Respond, record</text>
  <line x1="155" y1="120" x2="170" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="305" y1="120" x2="320" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="455" y1="120" x2="470" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="605" y1="120" x2="620" y2="120" stroke="#02375B" stroke-width="2"/>
  <rect x="60" y="215" width="320" height="170" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="220" y="250" text-anchor="middle" font-size="18" fill="#02375B" font-weight="bold">Revocation</text>
  <text x="220" y="285" text-anchor="middle" font-size="15" fill="#02375B">Changes the status of a credential</text>
  <text x="220" y="315" text-anchor="middle" font-size="15" fill="#02375B">Done by the issuer</text>
  <text x="220" y="345" text-anchor="middle" font-size="15" fill="#4F6576">A status record may stay</text>
  <rect x="420" y="215" width="320" height="170" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="580" y="250" text-anchor="middle" font-size="18" fill="#02375B" font-weight="bold">Deletion</text>
  <text x="580" y="285" text-anchor="middle" font-size="15" fill="#02375B">Removes personal data</text>
  <text x="580" y="315" text-anchor="middle" font-size="15" fill="#02375B">Follows a request or retention end</text>
  <text x="580" y="345" text-anchor="middle" font-size="15" fill="#4F6576">Exceptions may apply</text>
</svg>

**Worked example: A deletion request after a course**

*Context 1: a training provider.* A former learner emails the provider: "Please remove my certificate and everything you hold about me." The registry officer recognises this as an erasure request, logs it the same day and asks the learner to reply from the registered email address to confirm identity. The privacy contact searches the platform, the evidence store and the email archive. The public profile and the project files are deleted. A minimal award record is kept because the provider has a legal duty to keep records of accredited awards, and the provider explains this to the learner in its reply. The provider notes the request and outcome in its log.

*Context 2: a corporate academy.* An employee asks HR to delete a badge after changing roles. The HR privacy contact separates two questions. First, should the badge be revoked? The badge remains valid, so no. Second, should data be deleted? The employee's personnel file follows HR retention rules, but the badge on the employee's profile can be removed and the platform's access logs fall under their own retention period. HR explains this and offers the employee the option to hide the badge.

**Practice activity: Walk through a request**

Imagine this email: "I am a former learner and I want to know what you hold about me and I want my badge gone." Write a short response plan. List which rights are involved, the six process steps with names of roles in your organisation, and which of the two actions, revocation or deletion, you would consider. Note one case in which you might keep some data and explain why.

<details>
<summary>Facilitator notes</summary>

Role-play in groups of three: earner, registry officer, privacy contact. The earner sends an unclear request in everyday words. The registry officer must recognise it and pass it on. Debrief on how long it took to find all data locations. About 30 minutes.

</details>

### Check your understanding

**Question 1.** An earner writes: "Please tell me what data you have about me." What should the issuer do?

[( )] Ignore it, because it is not on an official form
[( )] Reply only if the earner uses the word "GDPR"
[(X)] Recognise it as an access request, log it, verify identity and respond within the legal deadline
[( )] Delete all the earner's data

****
Requests do not need a special form or legal wording. Staff must recognise a request in everyday language and start the process: log, verify identity, route, search, respond and record.
****

**Question 2.** What is the difference between revocation and deletion?

[( )] They are the same action
[( )] Revocation deletes data and deletion changes status
[(X)] Revocation changes a credential's status as valid or not, while deletion removes personal data from systems
[( )] Revocation is done by the earner and deletion by the verifier

****
Revocation is a status action by the issuer. Deletion is the removal of personal data. A revoked credential's status record may need to stay so that verifiers can see it is no longer valid.
****

**Question 3.** An earner asks for erasure, but the issuer has a legal duty to keep a record of accredited awards. What is the right approach?

[( )] Delete everything and ignore the duty
[( )] Refuse and not respond
[(X)] Delete what can be deleted, keep only what the duty requires, and explain the decision to the earner
[( )] Make the whole record public

****
The right to erasure has exceptions, including legal obligations. The issuer deletes what it can, keeps the minimum that the obligation requires and gives the earner a clear explanation.
****

**Question 4.** Which step comes right after logging an incoming earner request?

[( )] Deleting all data
[(X)] Verifying the identity of the person making the request
[( )] Sending the data to a third party
[( )] Closing the request

****
After recognising and logging a request, the issuer confirms the person's identity, using no more data than necessary, to avoid giving data to the wrong person.
****

## Third parties, platforms and transfers

### Who else touches the data

Few issuers run everything themselves. Credential data often reaches other organisations:

- a credential issuing platform or wallet provider
- a learning management system provider
- an assessment or proctoring service
- an email delivery service
- cloud hosting and backup providers
- verifiers, such as employers or other institutions
- AI services used for marking, summaries, matching or chat support

The GDPR distinguishes roles. A **controller** decides why and how personal data is processed. A **processor** processes data on behalf of the controller. Most issuers are controllers. Platform providers are often processors. When a provider acts as a processor, the issuer needs a written contract, called a data processing agreement, that sets out what the provider may do with the data and which security measures apply. In some cases two organisations decide together and are joint controllers, and they must agree on their respective responsibilities.

Choosing a platform is therefore also a data protection decision. Ask which data it collects, where it is stored, who can access it, which subprocessors it uses and how it supports deletion and export.

### Transfers outside the EU or EEA

The GDPR restricts transfers of personal data to countries outside the European Economic Area, unless a safeguard applies. Safeguards include adequacy decisions of the European Commission, standard contractual clauses and some other mechanisms. A transfer can happen without anyone moving files. Remote access to data from another country can count too.

Your task at this level is to recognise when a transfer may occur and to ask the right questions. The legal assessment belongs to your data protection officer or legal adviser.

<!-- VERIFY: Check the current state of adequacy decisions and transfer mechanisms before any statement about specific countries is added. -->

### Sending evidence or earner data to AI services

AI services are now common in education and HR tools. They can summarise evidence, suggest feedback, draft emails or answer earner questions. Sending evidence or earner data to an AI service is a disclosure to a third party and needs the same care as any other disclosure.

Questions to ask before sending data to an AI service:

- **Purpose and basis.** Does this use fit the purposes in our privacy notice and our legal basis? Is it a new purpose?
- **Role of the provider.** Is the provider a processor under a written agreement? Does it use our data to train its own models? If so, on what terms?
- **Minimisation.** Can we remove names and identifiers before sending? Does the task need the full evidence or only a part?
- **Location and transfers.** Where is the data processed and stored?
- **Retention.** How long does the provider keep inputs and outputs, and can we have them deleted?
- **Sensitive data.** Does the evidence contain special category data, data about children or data about third parties?
- **Human oversight.** If the AI output affects an earner, for example by influencing a grade, is a person involved in the decision? Rules on automated decisions may apply.
- **Transparency.** Have we told earners that AI services are used?

A simple rule is that staff do not paste earner data into public AI tools that the organisation has not approved. Publish an approved list and a short staff rule.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg" font-family="Open Sans, Arial, sans-serif">
  <title>Where credential data can travel</title>
  <desc>The issuer sits in the centre. Arrows lead to five recipients: a credential platform, an email service, a verifier, an AI service and cloud hosting. A label says that each arrow needs a purpose, a contract and a check of where data is processed.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <text x="400" y="40" text-anchor="middle" font-size="20" fill="#02375B" font-weight="bold">Where credential data can travel</text>
  <rect x="300" y="170" width="200" height="90" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="210" text-anchor="middle" font-size="16" fill="#02375B" font-weight="bold">Issuer</text>
  <text x="400" y="235" text-anchor="middle" font-size="14" fill="#02375B">controller of the data</text>
  <rect x="40" y="75" width="190" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="135" y="111" text-anchor="middle" font-size="15" fill="#02375B">Credential platform</text>
  <rect x="570" y="75" width="190" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="665" y="111" text-anchor="middle" font-size="15" fill="#02375B">Email service</text>
  <rect x="40" y="295" width="190" height="60" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="135" y="331" text-anchor="middle" font-size="15" fill="#02375B">Verifier, employer</text>
  <rect x="305" y="320" width="190" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="356" text-anchor="middle" font-size="15" fill="#02375B">AI service</text>
  <rect x="570" y="295" width="190" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="665" y="331" text-anchor="middle" font-size="15" fill="#02375B">Cloud hosting</text>
  <line x1="300" y1="190" x2="230" y2="125" stroke="#02375B" stroke-width="2"/>
  <line x1="500" y1="190" x2="570" y2="125" stroke="#02375B" stroke-width="2"/>
  <line x1="300" y1="245" x2="230" y2="305" stroke="#02375B" stroke-width="2"/>
  <line x1="400" y1="260" x2="400" y2="320" stroke="#02375B" stroke-width="2"/>
  <line x1="500" y1="245" x2="570" y2="305" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="420" text-anchor="middle" font-size="14" fill="#4F6576">Each arrow needs a purpose, a contract and a check of where data is processed</text>
</svg>

### When a DPIA is needed

A data protection impact assessment (DPIA) is a structured process to describe processing, assess risks to people and plan measures to reduce them. The GDPR requires a DPIA where processing is likely to result in a high risk to the rights and freedoms of people. Supervisory authorities publish lists of processing types that need one.

Signs that you should ask your data protection officer whether a DPIA is needed:

- large-scale processing of special category data
- systematic monitoring of people, for example proctoring by camera
- use of new technologies, including AI, to evaluate or score people
- automated decisions with significant effects on earners, such as pass or fail
- combining datasets in ways earners would not expect
- processing data about children or other vulnerable people
- a new platform that holds credentials for many people in several countries

Do the DPIA before the processing starts. A DPIA does not mean the project must stop. It shows what must change to make the processing acceptable.

<!-- VERIFY: Check the national supervisory authority's list of processing operations that require a DPIA for the countries where the organisation operates. -->

### Watching for change

Data protection rules are stable at their core, but the legal landscape around them can change. Proposed changes to data rules, known as the Digital Omnibus, are under discussion at EU level. Status as of November 2026; check before publishing. Issuers should follow official announcements and ask their data protection officer to flag changes that affect credential processes.

**Worked example: An AI tool for feedback and a proctoring service**

*Context 1: a university.* A programme team wants to use an AI service to draft feedback on written assignments. The team lead lists the data involved: student names, essays and sometimes personal stories. Using the questions in this module, the team sees that essays can contain health or family information and that the provider may store inputs. The team asks the data protection officer, who recommends a DPIA because the tool evaluates students and uses new technology on a large scale. Until the DPIA is complete, staff do not send student work to the tool, and the team trials it on sample texts written by staff.

*Context 2: a corporate academy.* An HR department plans to use an online proctoring service with camera monitoring for a certification exam taken by employees in several countries. The learning technology owner notes systematic monitoring, special sensitivity for video, and possible transfers outside the EEA. The department opens a DPIA, signs a data processing agreement with the provider and informs candidates in advance about what is recorded and how long it is kept.

**Practice activity: Screen a proposed tool**

Pick a tool your organisation uses or might use that handles credential data, for example a credential platform, an AI assistant or a proctoring service. Answer the eight AI questions above, adapted to the tool. List the controller and processor roles. Then tick any DPIA signs from the list that apply. Write one paragraph recommending whether to ask the data protection officer about a DPIA, and why.

<details>
<summary>Facilitator notes</summary>

Bring two tool descriptions, one low-risk and one high-risk, and let groups screen both. Compare the results. Return to the participants' data maps from the kick-off and mark which locations involve third parties. About 30 minutes.

</details>

### Check your understanding

**Question 1.** A credential platform provider processes earner data only on the issuer's instructions. In GDPR terms, what is the provider's usual role?

[( )] Data subject
[( )] Supervisory authority
[(X)] Processor, which needs a written data processing agreement with the issuer
[( )] Verifier

****
A processor handles personal data on behalf of the controller. The issuer, as controller, needs a written contract that sets out what the processor may do and which security measures apply.
****

**Question 2.** A staff member wants to paste earners' written reflections into a public AI chat tool that the organisation has not approved. What is the best response?

[( )] Allow it, because the tool is free
[( )] Allow it if names are in the text
[(X)] Do not send the data, and use only approved tools after checking purpose, provider role, minimisation, location and retention
[( )] Allow it for special category data only

****
Sending earner data to an AI service is a disclosure to a third party. It needs a purpose, a suitable agreement, minimisation and checks on location and retention. Unapproved public tools should not receive earner data.
****

**Question 3.** Which proposal is most likely to need a DPIA?

[( )] Printing certificates on paper
[( )] Adding the issue date to a credential
[(X)] Camera-based proctoring of exams for a large group of candidates in several countries
[( )] Updating the colour of the credential template

****
Systematic monitoring, sensitive video data and cross-border processing at scale are signs of high risk. A DPIA helps to assess and reduce the risks before the processing starts.
****

**Question 4.** When should a DPIA be carried out?

[( )] After the processing has started and complaints arrive
[(X)] Before the processing starts, so that risks can be reduced in the design
[( )] Only when a regulator asks
[( )] Only once the contract ends

****
A DPIA is a preventive tool. Doing it before processing starts allows the organisation to change the design, add safeguards or decide not to proceed.
****

## Assessment and badge

### Knowledge check

The final knowledge check has 10 scenario-based questions. Each question has four options and exactly one correct answer. The questions cover all four learning outcomes. Read each scenario, choose the best answer and read the explanation that follows.

**Question 1.** A registry reviews its systems for a credential programme. It finds these items: the earner's email address on the credential record, a recorded presentation held as evidence, and a log of verification requests with IP addresses. Which statement is correct?

[( )] Only the email address is personal data
[( )] Only the credential record contains personal data
[(X)] All three items can be personal data, in the credential, the evidence and the platform logs
[( )] None of the items is personal data because the credential is public

****
Personal data can sit in the credential, in the evidence and in platform logs. Email addresses, recordings of people and IP addresses can each relate to an identifiable person.
****

**Question 2.** A college stores a student's exam adjustment note in the same folder as the student's portfolio, which several assessors can open. What is the main issue?

[( )] The note is public data
[( )] The note is anonymous
[(X)] The note may contain special category data and needs stricter access control and handling
[( )] The note must be published with the credential

****
Information about a health condition can be special category data. It should be kept in a more restricted record and not mixed into evidence folders with wide access.
****

**Question 3.** A training provider issues certificates under a training contract. It now plans to display each learner's certificate on a public gallery. How should it treat the gallery?

[( )] As covered by the training contract, with no further decision
[( )] As allowed because the certificate is already issued
[(X)] As a separate purpose that needs its own legal basis, often consent that is easy to give and withdraw, and clear information
[( )] As a purpose that needs no information to the learner

****
Public display is a different purpose from issuing. It needs a suitable legal basis, often consent where the learner chooses, with plain information and an easy way to withdraw.
****

**Question 4.** An HR department wants to rely on employee consent for publishing individual badges on the company website. What is the best advice?

[( )] Consent from employees is always valid
[( )] Consent is never a legal basis
[(X)] Consent may not be freely given in an employment relationship, so consider aggregate publication or an employee-controlled choice
[( )] Publish first and ask later

****
An employee may feel unable to refuse an employer. Consent must be freely given, so HR teams look for alternatives such as publishing counts without names, or letting employees choose for their own profile.
****

**Question 5.** A verification page for a micro-credential currently shows the earner's full name, grade band, home town and programme office email address. The purpose is to let employers confirm the award. What should the issuer do under data minimisation?

[( )] Add more fields to build trust
[( )] Keep all fields because they are already public
[(X)] Show only what a verifier needs, such as award, issuer, date and status, and remove the other fields
[( )] Move all fields to a social media page

****
Data minimisation limits data to what is needed for the purpose. Confirming an award needs far fewer fields than the page shows.
****

**Question 6.** A university has no written retention schedule for evidence. Staff keep scripts and recordings indefinitely "in case". Which principle is at risk?

[( )] The right to portability
[( )] Purpose limitation only
[(X)] Storage limitation, which requires keeping personal data no longer than necessary for the purpose
[( )] Adequacy of the processor

****
Keeping data indefinitely without a defined need conflicts with storage limitation. The issuer should set, document and apply retention periods, taking legal requirements into account.
****

**Question 7.** An earner emails a corporate academy: "Please delete my badge and all my details." The academy has an obligation to keep a minimal record of mandatory safety training for a set period. What is the best response?

[( )] Delete everything immediately
[( )] Ignore the email because it is informal
[(X)] Treat it as an erasure request, delete what can be deleted, keep only the minimal record the obligation requires, and explain this to the earner
[( )] Revoke the badge and tell nobody

****
An informal email can be a valid request. The right to erasure has exceptions, such as legal obligations. The academy deletes what it can, keeps the minimum and explains its decision.
****

**Question 8.** An issuer issued a credential by mistake to the wrong person. Which action changes the credential's validity status?

[( )] Deleting the earner's email address
[( )] Sending a privacy notice
[(X)] Revoking the credential
[( )] Restricting processing of the platform logs

****
Revocation is the status action that marks a credential as no longer valid. Deletion removes personal data and does not by itself change status.
****

**Question 9.** A programme team plans to send student essays to an AI service to draft feedback. The service evaluates students and may keep inputs. What is the best next step?

[( )] Start immediately, because AI tools are common
[( )] Send only essays from students who agree informally
[(X)] Ask the data protection officer whether a DPIA is needed, and check provider role, minimisation, location and retention before sending any data
[( )] Send the essays after removing the course title

****
Evaluating people with new technology can mean high risk. A DPIA is assessed before processing starts, along with checks on provider role, minimisation, location and retention.
****

**Question 10.** Which situation most clearly points to a DPIA?

[( )] Changing the font on a credential template
[( )] Adding a help link to a credential page
[(X)] Introducing camera-based proctoring with video recording for a large group of candidates in several countries
[( )] Correcting a typo in a privacy notice

****
Systematic monitoring, video data, scale and cross-border processing are signs of likely high risk to people. A DPIA should be done before the processing starts.
****

### Rubric

| Criterion | Evidence of understanding | Linked outcome |
|---|---|---|
| Identifying personal data | Recognises personal data in credentials, evidence and platform logs, and spots special category data | 1 |
| Legal basis and purpose | Explains that each purpose needs a legal basis and matches common purposes to bases | 2 |
| Minimisation and retention | Explains data minimisation, storage limitation and a minimal record for verification | 2 |
| Earner rights and requests | Describes the rights, the request steps, and the difference between revocation and deletion | 3 |
| DPIA recognition | Recognises signs that a DPIA is needed and that it comes before processing | 4 |

### Pass rule

Pass mark: 8 correct answers out of 10 (80 per cent). You may retry the knowledge check. Read the explanations and revisit the module that matches the outcome you missed before trying again.

### Badge and evidence

On passing, you earn the badge "Data Protection Basics for Credential Issuers (Knowledge, L1)", alignment code ICSF-SECP-L1-K. The evidence submitted for the badge is the passed knowledge check. The badge states that you passed a knowledge check on these topics. It does not state that you are competent to carry out a job role.

<details>
<summary>Facilitator notes</summary>

Optional live element (45 minutes): a case clinic. Each group receives a short fictional credential programme and must produce a one-page summary: personal data found, purposes and legal bases, fields to remove, retention proposal, one request scenario and a DPIA screening result. Groups present in three minutes each. This activity is not part of the badge evidence.

</details>

## Sources and further reading

Status as of November 2026; check before publishing. Confirm the current version of each text and any amendments before use.

- Regulation (EU) 2016/679, the General Data Protection Regulation (GDPR), published in the Official Journal of the European Union and available through EUR-Lex.
- European Data Protection Board (EDPB): guidelines and recommendations on topics such as consent, data subject rights, controllers and processors, data protection by design and by default, and data protection impact assessments. Available from the EDPB website.
- National data protection supervisory authorities: guidance and lists of processing operations that require a DPIA in your country. Find your authority through the EDPB website.
- European Commission: information on the EU data protection rules and on international data transfers, including adequacy decisions.
- ICoBC Credentialing Skills Framework (ICSF), skill SECP "Security, privacy and data protection". Available from ICoBC at info@icobc.net.
- Digital Omnibus: proposals concerning changes to EU digital and data rules. Follow official announcements of the European Commission, and check the current status before relying on any change. <!-- VERIFY: Confirm the current status and content of the Digital Omnibus proposals before publishing. -->
