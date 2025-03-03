## Playbook Pages

- [Localization](https://common-voice.github.io/community-playbook/sub_pages/Localization.html): Translating project tools and material to be understood by contributors in their language 
- [Text Corpus](https://common-voice.github.io/community-playbook/sub_pages/text.html): Gathering, validating and processing public domain sentences               
- [Voice Corpus](https://common-voice.github.io/community-playbook/sub_pages/voice.html): Recording and validating voice clips to create a public domain dataset  
- [Communities](https://common-voice.github.io/community-playbook/sub_pages/communities.html): Connect with the variety of communities participating in Common Voice
- [Mobilization](https://common-voice.github.io/community-playbook/sub_pages/mobilization.html): Resources and tips for mobilizing your community                 
- [CC0 Waiver Process](https://common-voice.github.io/community-playbook/sub_pages/cc0waiver_process.html): How to secure a cc0 license for text corpus   

## 📝 Text corpus

### Our purpose

Collect or generate text corpus under public domain licence that can be read by people to facilitate their voice donations. Public domain texts are creative works that have no exclusive intellectual property rights. 

### Who we are

We are a community of text collectors and creators, always looking for places with text corpora we can extract and process so it can be transformed into short and simple sentences for people to read.

### What’s success

Generate as many sentences as possible in our languages. Having more sentences allows contributors to donate more hours of voice data.

* 5,000 sentences 	_allow_ 	5,5 hrs of voice
* 9,000 sentences 	_allow_ 	10 hrs of voice
* 90,000 sentences	_allow_ 	100 hrs of voice
* 1,800,000 sentences _allow_ 	2000 hrs of voice

⚠️ _You will need at least 5000 validated sentences to have your language enabled for voice contributions on our voice collection site._

### How to join

Anyone can join this community. Join our [discourse forums](https://discourse.mozilla.org/c/voice/) or our [matrix chat](https://chat.mozilla.org/#/room/#common-voice:mozilla.org), introduce yourself and jump into our sentence tools right away.

### What we do

#### **Sentence extraction**

We have developed [a tool to extract sentences](https://github.com/Common-Voice/cv-sentence-extractor) from large sources of public domain text, with a focus easy-to-read corpus and Wikipedia.

This is the easiest and fastest way to get more than a million sentences as soon as possible for your language.

<p style="text-align: right">
ℹ️ <em>Please read <a href="https://github.com/Common-Voice/cv-sentence-extractor#common-voice-sentence-extractor">the tool documentation</a> on how to generate specific rules for your language. </em></p>

⚠️ _Important: Due to legal reasons Mozilla needs to be the one running the final extraction, so please don’t do any manual processing to the resulting extraction during your tests. We can apply manual clean-up after the final version is generated by Mozilla._

🔨 _Skills required to help: Command line usage and git, familiar with regular expressions._

#### **Sentence collection**

We have also created a [sentence collection tool](https://commonvoice.mozilla.org/sentence-collector/#/) that allows contributors to collect and validate sentences created by the community. You can use this tool also to import and clean-up small-to-medium-sized public domain corpus you have found or collected.

ℹ️ _Please read [the collector how-to](https://commonvoice.mozilla.org/sentence-collector/#/how-to) before using this tool and check the [community guidelines on how to validate sentences](https://discourse.mozilla.org/t/discussion-of-new-guidelines-for-uploaded-sentence-validation/37718)_.

🔨 _Skills required to help: Strong grammar knowledge of the target language you are contributing to._

#### Bulk submission

If you know of a public domain corpus of sentences with more than 100k sentences, you can manually submit a pull request to add this as a bulk dataset. However, you will need to manually perform QA (quality assurance) to make sure the sentences are valid and high-quality.

[This Discourse post](https://discourse.mozilla.org/t/using-the-europarl-dataset-with-sentences-from-speeches-from-the-european-parliament/50184) has a more detailed guide for how to do manual QA, but in brief:

- You need 2-3 native speakers to review a random sample of sentences to verify their correctness
- The sentences should be spelled correctly.
- The sentences should be grammatically correct.
- The sentences should be speakable (also avoiding non-native uncommon words)
- Please share your reviewed sentences in txt. format

We're looking for less than 5% of error rate on the random sample. You can use [this tool](https://www.surveymonkey.com/mp/sample-size-calculator/) with a confidence level of 99% and a margin of error of 2% to determine the sample size you need to review.

Feel free to set up this QA however makes most sense for you, but here's a [sample Google Spreadsheets template](https://docs.google.com/spreadsheets/d/1dJpysfcwmUwR4oJuw5ttGcUFYLeTbmn50Fpufz9qx-8/edit#gid=0).

Once the review is complete, submit a pull request with the # of sentences submitted, a link to the manual QA results, and the % error rate. Here's [an example PR](https://github.com/mozilla/common-voice/pull/2873).

#### Flagging problematic sentences

If you notice sentences that need to be deleted, first check what the source of the sentence is. If the file that the sentence is located in is called `sentence-collector.txt`, that means it was automatically exported from Sentence Collector. In that case, please file an issue on the [Sentence Collector repo](https://github.com/Common-Voice/sentence-collector/) with a plaintext file of all of the problem sentences, with one sentence per line.

If the sentence is from a different source, you can file a pull request that modifies the text file directly. If possible, also attach a separate plaintext file that has all of the problem sentences, with one sentence per line.

### Automatic Translation 

Some language communities have used automatic translation of high-resource languages corpus' licensed under cc0 and adapted materials for cultural context in the language. After translating the texts, they have reviewed the sentences through the sentence collector. The Common Voice Team doesn't have a formal position on automatic translation for sentence collection. 

#### **Tooling development**

Contributors also develop, maintain and update the sentence extractor and collector code.

* Sentence Extractor: 🐞 [Open issues](https://github.com/Common-Voice/cv-sentence-extractor/projects/1?fullscreen=true) - 🔨 _Skills needed: Rust_
* Sentence Collector: 🐞 [Open issues](https://github.com/Common-Voice/sentence-collector/projects/2?fullscreen=true) - 🔨 _Skills needed: React, JavaScript, Node.js_

#### Collaborating with publishers of copyrighted works

We build relationships with organisations or individuals who would be happy to donate their text under a Public domain license. 

⚠️ _Important: Due to legal reasons Mozilla you will have to confirm the agreement with the copyright owner. This process is outlined on [cc0waiver_process page](https://common-voice.github.io/community-playbook/sub_pages/cc0waiver_process.html). 

### Roles

These are some roles you can take as part of this community.

* Text searcher - Find and connect with sources and organizations that have or are willing to donate text corpus under public domain licence.
* Text processor - Cleaning up the raw text corpus to apply [our sentences requirements](https://common-voice.github.io/sentence-collector/#/how-to).
* Text creator - Generate your own sentences and release them under public domain.
* Validator - Help validate and review existing cleaned-up sentences.
* Mobilizer - Help people in the community to get started and keep contributing.
* Developer - Develop, maintain and update the sentence tooling
* Linguist - Providing advice on grammatically or linguistic needs, for example, large corpus validation 

### Channels

* [Common Voice discourse](https://discourse.mozilla.org/c/voice/) category.
* [Common Voice matrix](https://chat.mozilla.org/#/room/#common-voice:mozilla.org) chat room.
* [Sentence Extractor matrix](https://chat.mozilla.org/#/room/#common-voice-sentence-extractor:mozilla.org) chat room.
* [Common Voice project announcements](https://discourse.mozilla.org/tags/c/voice/announcements).

💬 If your language already exists on Common Voice, make sure you [check and join the local discourse](https://voice.mozilla.org/about#get-involved) and matrix room. If that’s not the case, please create a new topic [on discourse](https://discourse.mozilla.org/c/voice/239) asking for one to be created.

