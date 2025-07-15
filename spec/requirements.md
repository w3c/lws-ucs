1.  <dfn>Globally Unique Identifiers</dfn> — Resources, including Entities and Storages, shall be uniquely identifiable globally. No two distinct Resources shall share the same Identifier (though a "collective" Resource with one Identifier may be comprised of several Resources, each with its own Identifier, and actions taken on the collective Resource can affect all the Resources which comprise the collective Resource). A Resource may be identifiable via multiple, distinct identifiers. 

    Issues: [#136](https://github.com/w3c/lws-ucs/issues/136), [#108](https://github.com/w3c/lws-ucs/issues/108)  
    Stories: Globally Unique Identifiers

2.  <dfn>Use of Service Providers</dfn> — The protocol shall provide a mechanism for Entities to delegate some functions to trusted Service Providers. Some interactions may require a trust relationship between Service Providers and Entities. In general, this should not impede the ability of an Entity to operate or self-host a service. Also, trust relationships are not transitive, in the sense that if an Entity trusts a Service Provider, e.g. an Identity Provider, it does not follow that another Service Provider the Entity interacts with, e.g. a Storage Provider, is under any obligation to trust said Identity Provider.

    Issues: [#127](https://github.com/w3c/lws-ucs/issues/127)  
    Stories: Trust Mechanism for Storage Providers

3.  <dfn>Control of Storages</dfn> — An Entity shall be able to control one or more Storages across one or more Storage Providers. A Storage shall have exactly one Controller.

    Issues: [#130](https://github.com/w3c/lws-ucs/issues/130)  
    Stories: Storage Ownership

4.  <dfn>Delegation of Control</dfn> — The system shall allow for an Entity to delegate control of a Storage to another Entity. Delegation could be temporary, i.e. have an expiration time, or not. An Entity shall be able to modify delegation at a later time, either by changing expiration or revoking it altogether.  
    Stories: Delegation of Control

5.  <dfn>Transfer of Control</dfn> — The protocol shall allow for an Entity to transfer, i.e. irrevocably reassign control of a Storage to another Entity.  
    Stories: Delegation of Control

6.  <dfn>Storage Portability</dfn> — The protocol shall allow for an Entity to port, i.e. move or transfer, the entire contents of a Storage from one Storage Provider to another. Once the move is complete, the previous Storage Provider shall be freed from any responsibility related to the Storage.

    Issues: [#140](https://github.com/w3c/lws-ucs/issues/140)  
    Stories: Portable Storage

7.  <dfn>Adding, Updating, Deleting Resources in Storage</dfn> — The protocol shall allow for Resources to be added, updated and/or deleted within a Storage by authorized Entities. In general the protocol shall allow for any type of resource to be stored in a Storage, however Storage Providers may impose certain limitations, such as of type or size.

    Issues: [#117](https://github.com/w3c/lws-ucs/issues/117), [#124](https://github.com/w3c/lws-ucs/issues/124)  
    Stories: Generic Storage

8.  <dfn>Data Sharing</dfn> — The protocol shall allow an Entity to grant access to a Resource it controls to another Entity. In other words, the first Entity may allow the other Entity to perform some operations (read, modify, remove...) on the Resource. Access grant could be temporary, i.e. have an expiration time, or not. The first Entity shall be able to modify delegation at a later time, either by changing the expiration time or revoking it altogether.

    Issues: [#27](https://github.com/w3c/lws-ucs/issues/27), [#118](https://github.com/w3c/lws-ucs/issues/118)  
    Stories: Sharing Access, Profile Sharing, Group Sharing, Health Record Access

9.  <dfn>Auditable Trail</dfn> — The protocol shall make it possible for an authorized Entity to access an auditable log of all access requests and grants to Resources and all read/write/delete of Resources.

    Issues: [#84](https://github.com/w3c/lws-ucs/issues/84)  
    Stories: Administrative Assistant, Legal Reporting, Health Record Access

10. <dfn>Serialization Format</dfn> — The protocol shall make it possible for data in a Storage to be serialized in a known format.  
    Stories: Data Integration, Personal Information Management

11. <dfn>Offline Access and Synchronization</dfn> — The protocol shall allow Entities to access and modify data even when disconnected from the network, with local changes synchronized to the online Storage once connectivity is restored. This includes providing strong guarantees against data corruption and robust conflict resolution to ensure data consistency after offline edits.  
    Stories: Offline Data Access, Storage Listening

12. <dfn>Resumable Large Data Transfers</dfn> — The protocol shall support efficient handling of large files and data streams, including the ability to resume interrupted uploads/downloads. This ensures that network or server interruptions do not force restarting an entire transfer, improving reliability for big file operations.

    Issues: [#18](https://github.com/w3c/lws-ucs/issues/18)  
    Stories: Large File Uploads

13. <dfn>Data Versioning</dfn> — The protocol shall support maintaining and retrieving previous versions of Resources. Authorized Entities should be able to recover or inspect earlier versions of data (including metadata and access control states) to enable undoing changes, auditing modifications, or recovering from accidental deletions. This helps ensure data durability and traceability over time.  
    Stories: Generic Storage

14. <dfn>Notification and Eventing</dfn> — The protocol shall provide a mechanism to notify relevant Entities of significant events, such as changes to Resources or updates to access permissions. For example, if access rights on a Resource change or new data is available, the affected parties can be alerted in a timely manner. Notification delivery may be real-time (e.g., push/SSE) or via queued channels (e.g., email or inbox), respecting user preferences and privacy.

    Issues: [#32](https://github.com/w3c/lws-ucs/issues/32), [#100](https://github.com/w3c/lws-ucs/issues/100), [#101](https://github.com/w3c/lws-ucs/issues/101)  
    Stories: Notifications for Permission Changes, Real-Time Notifications, Application Notifications

15. <dfn>Access Request Handling</dfn> — The protocol shall enable an Entity to request access to a Resource they are currently not authorized to use, and allow the Resource owner (or controller) to review and grant or deny such requests. There should be a standard way for a requester to signal a desire for access and for the owner to be notified and respond. This ensures that data owners can easily share data upon request without preemptively granting broad access.

    Issues: [#11](https://github.com/w3c/lws-ucs/issues/11), [#28](https://github.com/w3c/lws-ucs/issues/28), [#78](https://github.com/w3c/lws-ucs/issues/78), [#79](https://github.com/w3c/lws-ucs/issues/79), [#92](https://github.com/w3c/lws-ucs/issues/92)  
    Stories: Health Record Access

16. <dfn>Delegation of Access Rights</dfn> — Beyond whole-storage control delegation, the protocol shall allow an Entity who has certain access rights on a Resource to delegate a subset of those rights to another Entity, if permitted by the original owner. Such sub-delegation may be temporary or scoped, and the original grantor (or the Resource owner) shall be able to revoke or modify the delegated rights at any time.

    Issues: [#10](https://github.com/w3c/lws-ucs/issues/10), [#104](https://github.com/w3c/lws-ucs/issues/104)  
    Stories: Administrative Assistant, Health Record Access

17. <dfn>Contextual Access Control</dfn> — The access control mechanisms shall support context-aware policies. An Entity should be able to impose additional conditions on Resource access based on context such as time windows, location, or group membership status. For instance, a policy could allow access only during certain hours, or only if the requesting party is within a specific role or group at the time.

    Issues: [#17](https://github.com/w3c/lws-ucs/issues/17), [#65](https://github.com/w3c/lws-ucs/issues/65)  
    Stories: Context-Aware Access Policies

18. <dfn>Inter-User Communication</dfn> — The protocol shall provide a mechanism for users (or their agents/applications) to exchange messages or data directly via their Storages in a standardized way, enabling built-in collaboration without relying on external messaging services. For example, a user should be able to send a message, notification, or invite to another user's Storage (with appropriate authorization), and the receiving user's client can retrieve or be alerted to this message.

    Issues: [#22](https://github.com/w3c/lws-ucs/issues/22), [#99](https://github.com/w3c/lws-ucs/issues/99)  
    Stories: Universal Communication

19. <dfn>Search and Query</dfn> — The protocol shall support querying of data to help users and applications discover Resources based on content or metadata. It shall offer powerful search capabilities (e.g., full-text or attribute-based search) while enforcing access controls on results. To handle large result sets, the protocol shall provide features like pagination, filtering, and sorting of query results, and may support standard query languages (such as SPARQL) for advanced semantic queries over the data.

    Issues: [#45](https://github.com/w3c/lws-ucs/issues/45), [#103](https://github.com/w3c/lws-ucs/issues/103), [#152](https://github.com/w3c/lws-ucs/issues/152)  
    Stories: Search Functionality, Pagination & Filtering, SPARQL Queries

20. <dfn>Self-Descriptive and Discoverable APIs</dfn> — The protocol shall include means for clients to discover available capabilities and navigate a Storage's data and access control interfaces uniformly. This could be achieved via hypermedia controls or standard descriptors in responses (e.g., JSON-LD links indicating available actions or endpoints). Servers should provide a discoverable description of their supported protocol versions, extensions, or features.

    Issues: [#21](https://github.com/w3c/lws-ucs/issues/21), [#70](https://github.com/w3c/lws-ucs/issues/70)  
    Stories: Storage Description and Discovery

21. <dfn>End-to-End Encryption</dfn> — The protocol shall enable end-to-end encryption of data such that data stored or transmitted is unreadable to anyone except the authorized parties. Even Storage Providers or network intermediaries cannot decrypt the content (only the data owner and intended recipients can). End-to-end encryption should be achievable for data at rest and in transit, using standard algorithms.

    Issues: [#4](https://github.com/w3c/lws-ucs/issues/4), [#44](https://github.com/w3c/lws-ucs/issues/44)  
    Stories: End-to-End Encryption

22. <dfn>Data Integrity Verification</dfn> — The protocol shall incorporate mechanisms to ensure and verify the integrity of stored data. Authorized Entities should be able to detect if data has been tampered with or corrupted (whether at rest or in transit). For example, the system may use cryptographic hashes, signatures, or checksums so clients can confirm that a Resource retrieved from Storage is exactly as originally stored by the owner.  
    Stories: Legal Reporting

23. <dfn>Consent-Based Data Sharing</dfn> —
* The protocol shall provide a means to record and honor user consent for data sharing, including details on who, what, purpose, and duration.
* There shall be a verifiable, auditable record of consent (e.g., receipts or tokens) that is revocable, ensuring access removal upon withdrawal.

    Issues: [#141](https://github.com/w3c/lws-ucs/issues/141), [#81](https://github.com/w3c/lws-ucs/issues/81)  
    Stories: Consent-Based Sharing

24. <dfn>Legal Basis Enforcement</dfn> — The protocol shall support associating access control decisions with legal bases or policies. For example, implementers should be able to tag data access rules with specific legal grounds (such as "Consent – GDPR Article 6(1)(a)" or "Contract – GDPR Article 6(1)(b)"), and record these as metadata alongside audit trails.

    Issues: [#80](https://github.com/w3c/lws-ucs/issues/80), [#77](https://github.com/w3c/lws-ucs/issues/77)  
    Stories: Legal Grounds Support

25. <dfn>User-Centric Identity Management</dfn> — The protocol shall integrate with identity systems in a way that empowers users to control their credentials and identifiers. Users should be able to manage self-sovereign identities or locally stored credentials and authenticate to a Storage using an identity solution they trust, accommodating standards like decentralized identifiers or client-managed credentials.

    Issues: [#25](https://github.com/w3c/lws-ucs/issues/25), [#90](https://github.com/w3c/lws-ucs/issues/90), [#115](https://github.com/w3c/lws-ucs/issues/115), [#128](https://github.com/w3c/lws-ucs/issues/128)  
    Stories: Identity & Credentials Management

26. <dfn>Modern Authentication Methods</dfn> — The protocol shall support contemporary web authentication methods, such as passkeys or WebAuthn for passwordless login, "silent" non-interactive flows for scripts, and client-credentials or token-based auth for automation. All methods must result in a verified Entity identity recognized by the Storage.

    Issues: [#39](https://github.com/w3c/lws-ucs/issues/39), [#49](https://github.com/w3c/lws-ucs/issues/49)  
    Stories: Authentication Mechanisms

27. <dfn>Trusted Identity Providers</dfn> — The protocol shall enable Storage Providers to establish trust relationships with Identity Providers of their choosing, rather than blindly accepting any identity source. Trust is non-transitive: a Storage only accepts credentials from IdPs it explicitly trusts.

    Issues: [#129](https://github.com/w3c/lws-ucs/issues/129)  
    Stories: Trust Mechanism for Storage Providers

28. <dfn>Protocol Binding Independence</dfn> — The core data access and identity interactions shall be defined abstractly, decoupled from any single transport or encoding. While HTTP(S) is expected, the protocol's semantics must be mappable to alternative transports (e.g., gRPC, GraphQL over WebSocket, local IPC) without changing its fundamental model.

    Issues: [#24](https://github.com/w3c/lws-ucs/issues/24)  
    Stories: API Protocol Decoupling

29. <dfn>Service Integration Authentication</dfn> — The protocol shall support secure authentication and authorization flows suitable for server-to-server and backend service integration, such as mutual TLS, signed JWT-based service credentials, or scoped long-lived tokens, enabling trusted services to access user Storages without interactive login.

    Issues: [#40](https://github.com/w3c/lws-ucs/issues/40), [#92](https://github.com/w3c/lws-ucs/issues/92)  
    Stories: Backend Service Integration

30. <dfn>Scalable Storage Management</dfn> — The protocol shall permit flexible management of an Entity's data across multiple storage units or providers, allowing logical unification of disparate back-ends. Clients should experience a single coherent Storage view even if data is split or migrated across providers, supporting scenarios like jurisdictional partitioning or provider failover.

    Issues: [#110](https://github.com/w3c/lws-ucs/issues/110), [#136](https://github.com/w3c/lws-ucs/issues/136)  
    Stories: Storage Flexibility

31. <dfn>Performance and Scalability</dfn> — The protocol and its implementations shall be designed for high performance at scale. Access control checks and data operations should incur minimal overhead, and the design should allow batching, caching, and distributed/clustered deployments to meet typical web performance needs.

    Issues: [#72](https://github.com/w3c/lws-ucs/issues/72)  
    Stories: Performant Access Control

32. <dfn>Clear Error Messaging</dfn> — The protocol shall specify clear and standardized error messages for various failure conditions, including meaningful status codes and human-readable information indicating the cause and possible remediation.

    Issues: [#34](https://github.com/w3c/lws-ucs/issues/34)  
    Stories: Clear Error Messages

33. <dfn>Profile Management</dfn> — The protocol shall support Entities having multiple distinct Profiles (e.g., "work" vs. "personal"), each with its own identifiers, metadata namespaces and access-control rules, so that data can be selectively shared under different personas.  
    Stories: Profile Sharing

34. <dfn>Group-Based Access Control</dfn> — The protocol shall allow Controllers to define and manage Groups of Entities, apply access control rules at the group level, and propagate membership changes dynamically so that permissions update automatically as the group evolves.

    Issues: [#38](https://github.com/w3c/lws-ucs/issues/38), [#102](https://github.com/w3c/lws-ucs/issues/102)  
    Stories: Group Sharing

35. <dfn>View-Based Data Sharing</dfn> — The protocol shall enable Controllers to define and expose derived "views" of a Resource (e.g., filtered, aggregated or redacted subsets) such that recipients see only the authorized slice without duplicating the underlying data.

    Issues: [#63](https://github.com/w3c/lws-ucs/issues/63), [#106](https://github.com/w3c/lws-ucs/issues/106), [#116](https://github.com/w3c/lws-ucs/issues/116)  
    Stories: Sensor Data Sharing

36. <dfn>Federated Data Queries</dfn> — The protocol shall support Clients performing queries across multiple Storages (including SPARQL federation), aggregating and returning results transparently while enforcing each Storage's access controls.

    Issues: [#88](https://github.com/w3c/lws-ucs/issues/88)  
    Stories: Data Integration, SPARQL Queries

37. <dfn>Delivery Receipts</dfn> — The protocol shall provide a mechanism for sending verifiable receipts or acknowledgements when Resources (such as digital goods) are created, modified, delivered or accessed, ensuring publishers can confirm successful delivery or consumption.

    Issues: [#85](https://github.com/w3c/lws-ucs/issues/85)  
    Stories: Digital Goods Delivery

38. <dfn>Collaborative Editing</dfn> — The protocol shall define optional mechanisms (e.g. locking, optimistic concurrency or CRDT-based merges) to allow multiple Entities to co-author or edit the same Resource concurrently, with built-in conflict detection and resolution.

    Issues: [#146](https://github.com/w3c/lws-ucs/issues/146)  
    Stories: Semantic Collaboration

39. <dfn>Timeseries Data Support</dfn> — The protocol shall include primitives for storing, querying and aggregating timeseries Resources—supporting configurable resolution limits and multidimensional analysis for data like IoT streams or metrics.

    Issues: [#6](https://github.com/w3c/lws-ucs/issues/6)  
    Stories: Timeseries Storage

40. <dfn>Self-Describing Website Publication</dfn> — The protocol shall support publishing self-describing websites with persistent URIs directly from a Storage, enabling durable, interoperable content hosting.

    Issues: [#31](https://github.com/w3c/lws-ucs/issues/31)  
    Stories: Website Creation

41. <dfn>Network Flexibility</dfn> — The protocol shall ensure Storages remain accessible from home or mobile environments with dynamic IPs or NAT, providing mechanisms (e.g., NAT traversal, DNS aliasing) so connectivity isn't impeded by changing network endpoints.

    Issues: [#105](https://github.com/w3c/lws-ucs/issues/105), [#68](https://github.com/w3c/lws-ucs/issues/68)  
    Stories: Home Access

42. <dfn>Bring-Your-Own-Data Apps</dfn> — The protocol shall enable third-party applications to store, read, update, and delete their data within user-managed Storages, and to discover available Storage capabilities, so that users retain data ownership and sovereignty over app-generated content.

    Issues: [#12](https://github.com/w3c/lws-ucs/issues/12), [#120](https://github.com/w3c/lws-ucs/issues/120)  
    Stories: Bring-Your-Own-Data Apps

43. <dfn>Profile Interaction UI</dfn> — The protocol shall define a standard method for clients to fetch and display an Entity's profile (e.g., WebID), along with supported actions (follow, message, share), so users can engage seamlessly with contacts.

    Issues: [#47](https://github.com/w3c/lws-ucs/issues/47), [#48](https://github.com/w3c/lws-ucs/issues/48)  
    Stories: WebID Profile Interaction

44. <dfn>Personal Data Projection</dfn> — The protocol shall support projection or transformation of personal data into formats consumable by non-LWS applications (e.g., JSON, vCard), without duplicating underlying resources, to prevent data silos.

    Issues: [#2](https://github.com/w3c/lws-ucs/issues/2)  
    Stories: Personal Information Management
