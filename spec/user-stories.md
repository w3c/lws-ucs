## Functional Stories

### <dfn>Generic Storage</dfn>

Bob wants to store and organize his data in a `[=storage=]` available online, so that data could be accessed from any device, any location, at any time. Bob wants to be free to store any type of resource in the `[=storage=]`. Bob wants his `[=storage=]` to allow for resources to be added, updated and/or deleted.

### <dfn>Portable Storage</dfn>

Bob wants the ability and choice to host the `[=storage=]` himself, or delegate the hosting to a `[=storage provider=]`. The `[=storage provider=]` may impose certain limitations, such as of type or size, and Bob may accept that if informed in advance. Bob also wants the ability to move (aka port) his `[=storage=]` to another `[=storage provider=]` as desired, without loosing any access to existing data or metadata, so that Bob is not dependent in perpetuity on one `[=storage provider=]`.

Porting a `[=storage=]` from one provider to another should work the same even when Bob hosts the `[=storage=]` himself. In that situation Bob acts as `[=storage provider=]` as well. 

### <dfn>Sharing Access</dfn>

As an author with authoring permission, Guinan wants to use the sharing interface of her authoring tool to manage access permissions to her article, so that Deanna can review, Seven-of-Nine can co-edit, and Torres can view the progress. All `[=user=]`(s), Guinan, Deanna, Seven-of-Nine and Torres can identify themselves within the authoring tool using their personal online identities.

The sharing interface of the protocl shall ensure that each `[=user=]` receives the appropriate access without confusion. The protocol shall handle updates to access permissions and determine whether changes should trigger notifications to the target `[=user=]`(s).

### <dfn>Profile Sharing</dfn>

Alice wants to maintain and manage multiple profiles and have fine grained choice over who can see what profile, so that she can maintain her privacy. Alice wants to know and trust Bob's identity, the `[=user=]` she shares her data with, so that Mallory, a malicious actor could not impersonate Bob and gain access to her data.

### Administrative Assistant

As a Manager I want my administrative Assistant to exercise some, but not all, of my permissions, such as updating my calendar and screening my email, so that I don't have to waste my time on these matters. Manager spends a lot of time scheduling appointments and dealing with unimportant emails. Common permission infrastructure, such a Role-Based, Attribute-Based, or Policy-Based access control, doesn't provide sufficient flexibility for Manager to offload some of this work to Assistant and Assistant to offload some of that work to others.

See also https://github.com/w3c/lws-ucs/issues/10


### Large HTTP uploads

As a `user`,
I want to upload large files that may or may/not complete due to network and/or server issues.  Further, for very large uploads also knowing what percentage of a file(s) that is uploaded is handy to have as both user and developer.

See also https://github.com/w3c/lws-ucs/issues/18


#### References:

- [[[RESUMABLE_UPLOADS]]]


## Non-Functional Stories

## Technical Stories

## Spike Stories

