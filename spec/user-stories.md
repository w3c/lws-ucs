## Functional Stories

### <dfn>Generic Storage</dfn>

Bob wants to store and organize his data in a `[=storage=]` available online, so that data can be accessed from any device, any location, at any time. Bob wants to be free to store any type of resource in the `[=storage=]`. Bob wants his `[=storage=]` to allow for resources to be added, updated, and/or deleted.

### <dfn>Portable Storage</dfn>

Bob wants the ability and choice to host the `[=storage=]` himself, or delegate the hosting to a `[=storage provider=]`. A `[=storage provider=]` may impose certain limitations, such as resource type or size, and Bob may accept that if informed in advance. Bob also wants the ability to move (a/k/a port) his `[=storage=]` to another `[=storage provider=]` as desired, without losing any access to existing data or metadata, so that Bob is not dependent in perpetuity on one `[=storage provider=]`.

Porting a `[=storage=]` from one provider to another should work the same even when Bob hosts the `[=storage=]` himself. In that situation Bob also acts as `[=storage provider=]`. 

### <dfn>Sharing Access</dfn>

As an author with authoring permission, Guinan uses the sharing interface of her authoring tool to manage access to her article, so that Deanna can review, Seven-of-Nine can co-edit, and Torres can view the progress. All `[=user=]`(s) — Guinan, Deanna, Seven-of-Nine, and Torres — have personal online identities that can be used to assign these permissions.

The sharing interface of the protocol shall ensure that each `[=user=]` receives the appropriate access without confusion. The protocol shall handle updates to access permissions, and determine whether changes should trigger notifications to the target `[=user=]`(s).

### <dfn>Profile Sharing</dfn>

Alice wants to maintain and manage multiple profiles and have fine grained choice over who can see which profile(s), so that she can maintain her privacy. Alice wants to know and trust Bob's identity, the `[=user=]` she shares her data with, so that Mallory, a malicious actor, cannot impersonate Bob and gain access to her data.

Charlie learns about Alice's profile and tries to access it from his business card management application called SolidRolodex. He's not able to see it, because he was not yet granted access. Charlie needs a way to request access to Alice's profile from his app. Once Alice receives and approves Charlie's request, he will be able to access and see the data.

### <dfn>Group Sharing</dfn>

Alice is organizing a conference and stores a calendar for the conference in a Storage. Alice wants to share the calendar with the whole group of participants to the conference. The group of participants changes all the time during the registration process, new participants register and some drop out. Alice does not want to have to update the sharing grants every time the group composition changes.

Some of the participants are also speakers at the conference. They will need elevated permissions, such the ability to update the description of their presentation or upload and attach slides.

### <dfn>Heart Patient</dfn>

Frank is a heart patient and is measuring his heart rate and blood pressure from home. He does so every morning and evening. After moving to a new home in a different region/country, he wants a local cardiologist to have a look at his measurements to gain insights into his current condition and progress.

### <dfn>General Practitioner</dfn>

Over the last years Bob has accumulated comprehensive health data in his storage. He wants to share this data with his general practitioner, whom can change during his lifetime.

### <dfn>Administrative Assistant<dfn>

Charlie is the keynote speaker at the conference organized by Alice. Erin is his administrative assistant. Charlie wants to delegate the access granted to him by Alice to Erin so that she can make updates on his behalf. Charlie wants to delgate some, but not all, of his permissions, to Erin.

### <dfn>Offline Data</dfn>

Bob wants his storage to be available offline on his own device. He uses tools that access data in storages controlled either by himself or other trusted entities. Bob is sometimes disconnected from the internet, but would like to use his tools, so he needs local copies of his data or data shared with him. Bob would like data to be read-only at the very least, but, ideally, writable as well and synchronized once he regains internet connection. For the data available offline, Bob wants some strong guarantees that the data was not corrupted.

### Large HTTP uploads

As a `user`, I want to upload large files that may or may/not succeed in total due to network and/or server issues.  Further, knowing what percentage of a large file was successfully transferred can be handy to have as both user and developer.

See also https://github.com/w3c/lws-ucs/issues/18


#### References:

- [[[RESUMABLE_UPLOADS]]]


## Non-Functional Stories

## Technical Stories

## Spike Stories

