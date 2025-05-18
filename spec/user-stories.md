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

### <dfn>Offline Data</dfn>

Bob wants his storage to be availabel offline on his own device. He uses tools that access data in storages controlled either by himself or other trusted entity. Bob is sometimes disconnected from the internet, but would like to use his tools, so a local copy of his data or data shared with him would help. Bob would like data to be read-only at the very least, but, ideally, writable as well and synchronized once he regains internet connection. For the data available offline, Bob wants some strong guarantees that the data was not corrupted.

### Administrative Assistant

As a Manager, I want my administrative Assistant to be able to exercise some, but not all, of my permissions, such as updating my calendar and screening my email, so that I don't have to waste my time on these matters. A Manager spends a lot of time scheduling appointments and dealing with unimportant email. Common permission infrastructure, such a Role-Based, Attribute-Based, or Policy-Based access control, as commonly deployed today, doesn't provide sufficient flexibility for a Manager to offload some of this work to an Assistant nor for an Assistant to offload some of that work to others.

See also https://github.com/w3c/lws-ucs/issues/10


### Large HTTP uploads

As a `user`,
I want to upload large files that may or may/not succeed in total due to network and/or server issues.  Further, knowing what percentage of a large file was successfully transferred can be handy to have as both user and developer.

See also https://github.com/w3c/lws-ucs/issues/18


#### References:

- [[[RESUMABLE_UPLOADS]]]


## Non-Functional Stories

## Technical Stories

## Spike Stories

