
## Functional Stories

### Data Management

- <dfn>Generic Storage</dfn>
  **As a** user, **I want** a format-agnostic online storage system that supports any type of [resource](../glossary.md#resource), **so that** I can perform Create, Read, Update, and Delete (CRUD) — including metadata and access-control modifications, as well as recovering previous versions—from any device at any time.  
  *Context:* This ensures seamless data management across devices, empowering users with full control over their resources.  
  *Issues:* [#117](https://github.com/w3c/lws-ucs/issues/117), [#97](https://github.com/w3c/lws-ucs/issues/97), [#60](https://github.com/w3c/lws-ucs/issues/60), [#63](https://github.com/w3c/lws-ucs/issues/63), [#62](https://github.com/w3c/lws-ucs/issues/62), [#69](https://github.com/w3c/lws-ucs/issues/69)

- <dfn>Portable Storage</dfn>
  **As a** user, **I want** the ability to self-host my storage or switch between providers without losing my data, **so that** I retain data sovereignty and can withstand provider outages or migrations without data loss.  
  *Context:* Portability prevents vendor lock-in and enhances data sovereignty.  
  *Issues:* [#30](https://github.com/w3c/lws-ucs/issues/30), [#58](https://github.com/w3c/lws-ucs/issues/58), [#140](https://github.com/w3c/lws-ucs/issues/140), [#61](https://github.com/w3c/lws-ucs/issues/61)

- <dfn>Offline Data Access</dfn>
  **As a** user, **I want** to access and modify my data offline, with automatic synchronization upon reconnection, **so that** I can work without a network and avoid data corruption or conflicts.  
  *Context:* Offline support is vital for users in areas with unreliable connectivity.  
  *Issues:* [#138](https://github.com/w3c/lws-ucs/issues/138), [#64](https://github.com/w3c/lws-ucs/issues/64), [#65](https://github.com/w3c/lws-ucs/issues/65), [#67](https://github.com/w3c/lws-ucs/issues/67)

- <dfn>Large File Uploads</dfn>
  **As a** user, **I want** to upload large files with resumable uploads, **so that** interruptions don’t force me to restart the entire transfer.  
  *Context:* This improves usability for managing large media or data files.  
  *Issues:* [#18](https://github.com/w3c/lws-ucs/issues/18)

### Access Control and Sharing

- <dfn>Sharing Access</dfn>
  **As a** data owner, **I want** to grant and revoke fine-grained permissions on my resources, **so that** collaborators have appropriate access and receive notifications when their permissions change.  
  *Context:* Granular control ensures secure and tailored data sharing.  
  *Issues:* [#7](https://github.com/w3c/lws-ucs/issues/7), [#27](https://github.com/w3c/lws-ucs/issues/27),  [#116](https://github.com/w3c/lws-ucs/issues/116), [#148](https://github.com/w3c/lws-ucs/issues/148), [#120](https://github.com/w3c/lws-ucs/issues/120), [#98](https://github.com/w3c/lws-ucs/issues/98)

- <dfn>Notifications for Permission Changes</dfn>
**As a collaborator**, **I want** to receive notifications when my permissions on a resource are granted, revoked, or modified, so that I am informed about changes to my access rights in a timely manner.
Context: Timely notifications help collaborators stay updated on their access to shared resources, enhancing collaboration and security.
*Issues:* [#116](https://github.com/w3c/lws-ucs/issues/116), [#78](https://github.com/w3c/lws-ucs/issues/78)

- <dfn>Profile Sharing</dfn>
  **As a** user, **I want** to maintain multiple profiles with distinct access controls, **so that** I can share specific information while keeping other data private.  
  *Context:* Multiple profiles support different personas or contexts (e.g., work vs. personal).  
  *Issues:* [#29](https://github.com/w3c/lws-ucs/issues/29), [#57](https://github.com/w3c/lws-ucs/issues/57)

- <dfn>Group Sharing</dfn>
  **As a** user, **I want** to share data with dynamic groups (e.g., event attendees), **so that** membership and permissions update automatically as the group evolves.  
  *Context:* This simplifies access management for temporary or changing collaborations.  
  *Issues:* [#38](https://github.com/w3c/lws-ucs/issues/38), [#102](https://github.com/w3c/lws-ucs/issues/102)

- <dfn>Administrative Assistant</dfn>
  **As a** user, **I want** to delegate specific permissions to an assistant, with audit logs tracking their actions, **so that** they can manage my data securely on my behalf.  
  *Context:* Delegation aids users needing assistance while maintaining oversight.  
  *Issues:* [#10](https://github.com/w3c/lws-ucs/issues/10), [#104](https://github.com/w3c/lws-ucs/issues/104), [#118](https://github.com/w3c/lws-ucs/issues/118)

- <dfn>Context-Aware Access Policies</dfn>
  **As an** administrator, **I want** to enforce access policies based on contextual factors like time or geolocation or relative location (near Bob), **so that** access to data adapts dynamically to real-world conditions.  
  *Context:* Context-aware policies enhance security and flexibility.  
  *Issues:* [#17](https://github.com/w3c/lws-ucs/issues/17), [#147](https://github.com/w3c/lws-ucs/issues/147), [#94](https://github.com/w3c/lws-ucs/issues/94)

- <dfn>Health Record Access</dfn>
  **As a** patient, **I want** to share specific health records with an AI assistant using delegated authorization, **so that** I can get a second opinion with audit logs ensuring accountability.  
  *Context:* This supports secure, audited health data sharing for informed decisions.  
  *Issues:* [#11](https://github.com/w3c/lws-ucs/issues/11), [#46](https://github.com/w3c/lws-ucs/issues/46), [#54](https://github.com/w3c/lws-ucs/issues/54)

### Collaboration and Communication

- <dfn>Meeting Scheduling</dfn>
  **As a** user, **I want** to schedule meetings directly through my storage, with conflict detection for online and offline scenarios, **so that** I avoid double-booking.  
  *Context:* Integrated scheduling boosts productivity and coordination.  
  *Issues:* [#3](https://github.com/w3c/lws-ucs/issues/3), [#42](https://github.com/w3c/lws-ucs/issues/42)

- <dfn>Real-Time Notifications</dfn>
  **As a** collaborator, **I want** real-time notifications when resources I access are updated, **so that** I stay informed without manual checks.  
  *Context:* Timely updates enhance collaboration efficiency.  
  *Issues:* [#32](https://github.com/w3c/lws-ucs/issues/32), [#79](https://github.com/w3c/lws-ucs/issues/79)

- <dfn>Application Notifications</dfn>
  **As a** user, **I want** email or web push notifications for storage activity, **so that** I remain aware of important events.  
  *Context:* Notifications keep users engaged with their data.  
  *Issues:* [#100](https://github.com/w3c/lws-ucs/issues/100)

- <dfn>Universal Communication</dfn>
  **As a** user, **I want** direct messaging channels with other storage owners, **so that** I can collaborate seamlessly within the platform.  
  *Context:* Built-in communication strengthens user interaction.  
  *Issues:* [#99](https://github.com/w3c/lws-ucs/issues/99), [#22](https://github.com/w3c/lws-ucs/issues/22)

- <dfn>Polling</dfn>
  **As a** user, **I want** to create and manage polls within my storage, **so that** I can gather opinions and feedback from others.  
  *Context:* Polls support decision-making and community engagement.  
  *Issues:* [#144](https://github.com/w3c/lws-ucs/issues/144)

- <dfn>Semantic Collaboration</dfn>
  **As a** user, **I want** to co-author structured content with others using permanent URIs and flexible permissions, **so that** collaboration is efficient and traceable.  
  *Context:* This enables advanced use cases like shared knowledge bases.  
  *Issues:* [#146](https://github.com/w3c/lws-ucs/issues/146), [#98](https://github.com/w3c/lws-ucs/issues/98)

### Application Integration

- <dfn>Personal Information Management</dfn>
  **As a** user, **I want** to manage my personal data in my storage and integrate it with non-Solid apps via some data transformation, **so that** I can use various apps without creating data silos.  
  *Context:* This promotes interoperability and user control.  
  *Issues:* [#2](https://github.com/w3c/lws-ucs/issues/2)

- <dfn>Bring-Your-Own-Data Apps</dfn>
  **As an** app developer, **I want** my applications to store data in user's storage, with support for CRUD operations and store discovery, **so that** users retain ownership and control of their data.  
  *Context:* This shifts data ownership from apps to users.  
  *Issues:* [#12](https://github.com/w3c/lws-ucs/issues/12), [#120](https://github.com/w3c/lws-ucs/issues/120)

- <dfn>Digital Goods Delivery</dfn>
  **As a** user, **I want** secure delivery of digital goods (e.g., software, media) with confirmation receipts, **so that** providers can deliver assets with minimal intervention.  
  *Context:* This ensures reliable digital product delivery.  
  *Issues:* [#14](https://github.com/w3c/lws-ucs/issues/14)

- <dfn>Data Integration</dfn>
  **As an** app developer, **I want** a standardized API to combine data from multiple sources, **so that** integrating diverse datasets is straightforward and efficient.  
  *Context:* Simplified integration reduces development complexity.  
  *Issues:* [#26](https://github.com/w3c/lws-ucs/issues/26), [#53](https://github.com/w3c/lws-ucs/issues/53), [#88](https://github.com/w3c/lws-ucs/issues/88), [#106](https://github.com/w3c/lws-ucs/issues/106)

- <dfn>Business Data Access</dfn>
  **As a** business user, **I want** clear enforcement rules for data sharing, **so that** enterprise integrations comply with organizational policies.  
  *Context:* This supports secure enterprise use cases.  
  *Issues:* [#27](https://github.com/w3c/lws-ucs/issues/27), [#28](https://github.com/w3c/lws-ucs/issues/28)

### Advanced Features

- <dfn>Timeseries Storage</dfn>
  **As a** user, **I want** to store timeseries data with resolution limits and multidimensional analysis support, **so that** I can efficiently analyze trends over time.  
  *Context:* This is critical for applications like IoT or analytics.  
  *Issues:* [#6](https://github.com/w3c/lws-ucs/issues/6)

- <dfn>Sensor Data Sharing</dfn>
  **As a** user, **I want** to share sensor data at varying levels of granularity without duplication, **so that** consumers receive only the detail they need.  
  *Context:* Efficient sharing reduces resource usage.  
  *Issues:* [#8](https://github.com/w3c/lws-ucs/issues/8)

- <dfn>Legal Reporting</dfn>
  **As a** data provider, **I want** verifiable proof of data sharing to support audit compliance, **so that** I can meet legal obligations even after access is revoked.  
  *Context:* This ensures transparency and accountability.  
  *Issues:* [#9](https://github.com/w3c/lws-ucs/issues/9)

- <dfn>Search Functionality</dfn>
  **As a** user, **I want** powerful search capabilities with contextual awareness and security enforcement, **so that** I can find relevant resources quickly and safely.  
  *Context:* Effective search is essential for large datasets.  
  *Issues:* [#152](https://github.com/w3c/lws-ucs/issues/152), [#87](https://github.com/w3c/lws-ucs/issues/87)

- <dfn>Pagination & Filtering</dfn>
  **As a** user, **I want** efficient pagination, filtering, and ordering of search results, **so that** I can navigate large datasets easily.  
  *Context:* These features enhance data usability.  
  *Issues:* [#103](https://github.com/w3c/lws-ucs/issues/103)

- <dfn>SPARQL Queries</dfn>
  **As a** power user, **I want** support for SPARQL queries to perform complex searches and data analysis, **so that** I can extract insights from linked data.  
  *Context:* SPARQL enables advanced semantic web queries.  
  *Issues:* [#45](https://github.com/w3c/lws-ucs/issues/45)

- <dfn>Website Creation</dfn>
  **As a** user, **I want** to publish self-describing websites with persistent URIs, **so that** my content remains accessible and interoperable over time.  
  *Context:* This supports durable web publishing.  
  *Issues:* [#31](https://github.com/w3c/lws-ucs/issues/31)

- <dfn>Home Access</dfn>
  **As a** user, **I want** to access my storage from home devices with dynamic IPs, **so that** connectivity issues don’t prevent me from using my data.  
  *Context:* This ensures accessibility in home environments.  
  *Issues:* [#105](https://github.com/w3c/lws-ucs/issues/105), [#68](https://github.com/w3c/lws-ucs/issues/68)

- <dfn>Contextual Interactions</dfn>
  **As a** user, **I want** context-aware display of interactions alongside content, **so that** I can understand permissions and history intuitively.  
  *Context:* This improves user understanding of data interactions.  
  *Issues:* [#55](https://github.com/w3c/lws-ucs/issues/55)

- <dfn>WebID Profile Interaction</dfn>
  **As a** user, **I want** clicking a WebID to display profiles and available actions, **so that** I can engage with contacts effortlessly.  
  *Context:* This enhances social and professional interactions.  
  *Issues:* [#48](https://github.com/w3c/lws-ucs/issues/48), [#47](https://github.com/w3c/lws-ucs/issues/47)

- <dfn>Storage Listening</dfn>
  **As an** app developer, **I want** offline monitoring of storage changes, **so that** my applications stay synchronized even without connectivity.  
  *Context:* This supports robust offline app functionality.  
  *Issues:* [#101](https://github.com/w3c/lws-ucs/issues/101)

---

## Non-Functional Stories

### Security and Privacy

- <dfn>End-to-End Encryption</dfn>
  **As a** user, **I want** end-to-end encryption for all data storage and transfers, **so that** only authorized parties can decrypt and access my information.  
  *Context:* Encryption ensures data confidentiality.  
  *Issues:* [#4](https://github.com/w3c/lws-ucs/issues/4), [#44](https://github.com/w3c/lws-ucs/issues/44), [#73](https://github.com/w3c/lws-ucs/issues/73), [#74](https://github.com/w3c/lws-ucs/issues/74), [#75](https://github.com/w3c/lws-ucs/issues/75), [#76](https://github.com/w3c/lws-ucs/issues/76)

- <dfn>Consent-Based Sharing</dfn>
  **As a** user, **I want** verifiable consent mechanisms with audit trails for data sharing, **so that** I can ensure compliance with privacy regulations.  
  *Context:* Consent management supports ethical data practices.  
  *Issues:* [#141](https://github.com/w3c/lws-ucs/issues/141), [#80](https://github.com/w3c/lws-ucs/issues/80), [#81](https://github.com/w3c/lws-ucs/issues/81), [#82](https://github.com/w3c/lws-ucs/issues/82), [#83](https://github.com/w3c/lws-ucs/issues/83), [#84](https://github.com/w3c/lws-ucs/issues/84), [#85](https://github.com/w3c/lws-ucs/issues/85), [#86](https://github.com/w3c/lws-ucs/issues/86)

- <dfn>Legal Grounds Support</dfn>
  **As a** compliance officer, **I want** to define access policies based on legal grounds (e.g., GDPR), **so that** data sharing adheres to regulatory requirements.  
  *Context:* This ensures global compliance readiness.  
  *Issues:* [#80](https://github.com/w3c/lws-ucs/issues/80), [#141](https://github.com/w3c/lws-ucs/issues/141), [#77](https://github.com/w3c/lws-ucs/issues/77)

### Performance and Usability

- <dfn>Storage Ownership</dfn>
  **As a** user, **I want** ownership assigned upon storage creation, **so that** I have full control from the outset.  
  *Context:* Immediate ownership clarifies user authority.  
  *Issues:* [#43](https://github.com/w3c/lws-ucs/issues/43)

- <dfn>Performant Access Control</dfn>
  **As a** user, **I want** access control mechanisms that are responsive and scalable, **so that** the system performs well even under heavy load.  
  *Context:* Performance is critical for large-scale use.  
  *Issues:* [#72](https://github.com/w3c/lws-ucs/issues/72), [#153](https://github.com/w3c/lws-ucs/issues/153), [#71](https://github.com/w3c/lws-ucs/issues/71)

- <dfn>Clear Error Messages</dfn>
  **As a** user, **I want** error messages that are clear and actionable, **so that** I can resolve issues quickly and without frustration.  
  *Context:* Good error handling enhances user experience.  
  *Issues:* [#34](https://github.com/w3c/lws-ucs/issues/34)

---

## Technical Stories

### Identity Authentication and Trust

- <dfn>Identity & Credentials Management</dfn>
  **As a** user, **I want** to manage my identities and credentials locally, **so that** I control my authentication process directly from my device.  
  *Context:* Local management boosts security and autonomy.  
  *Issues:* [#25](https://github.com/w3c/lws-ucs/issues/25), [#90](https://github.com/w3c/lws-ucs/issues/90), [#115](https://github.com/w3c/lws-ucs/issues/115), [#153](https://github.com/w3c/lws-ucs/issues/153), [#128](https://github.com/w3c/lws-ucs/issues/128)

- <dfn>Authentication Mechanisms</dfn>
  **As a** user, **I want** support for modern authentication methods like passkeys, silent authentication, and script-friendly options, **so that** I can authenticate securely across diverse scenarios.  
  *Context:* Flexible authentication meets varied user needs.  
  *Issues:* [#39](https://github.com/w3c/lws-ucs/issues/39), [#41](https://github.com/w3c/lws-ucs/issues/41), [#49](https://github.com/w3c/lws-ucs/issues/49), [#50](https://github.com/w3c/lws-ucs/issues/50), [#51](https://github.com/w3c/lws-ucs/issues/51), [#114](https://github.com/w3c/lws-ucs/issues/114), [#162](https://github.com/w3c/lws-ucs/issues/162), [#129](https://github.com/w3c/lws-ucs/issues/129), [#130](https://github.com/w3c/lws-ucs/issues/130), [#136](https://github.com/w3c/lws-ucs/issues/136)

- <dfn>Trust Mechanism for Storage Providers</dfn>
  **As a** Storage Provider, **I want** a mechanism to trust Identity Providers for authenticating entities, **so that** I can ensure only authenticated and authorized entities access the storage.  
  *Context:* This trust relationship is crucial for maintaining security in a decentralized system where multiple Identity Providers may be involved.  
  *Issues:* [#129](https://github.com/w3c/lws-ucs/issues/129)

### API and Protocol Flexibility

- <dfn>API Protocol Decoupling</dfn>
  **As a** developer, **I want** APIs decoupled from HTTP, **so that** I can build local-first applications or use alternative protocols like gRPC or GraphQL.  
  *Context:* Decoupling enhances development flexibility.  
  *Issues:* [#24](https://github.com/w3c/lws-ucs/issues/24)

- <dfn>Backend Service Integration</dfn>
  **As a** service provider, **I want** secure authentication methods like mTLS or simpler alternatives for backend services, **so that** integration with LWS is seamless and secure.  
  *Context:* This ensures reliable backend connectivity.  
  *Issues:* [#40](https://github.com/w3c/lws-ucs/issues/40), [#56](https://github.com/w3c/lws-ucs/issues/56), [#92](https://github.com/w3c/lws-ucs/issues/92)

- <dfn>Storage Description and Discovery</dfn>
  **As a** user or application, **I want** to retrieve metadata about available storage and service capabilities, **so that** I can configure interactions appropriately and adapt to different storage behaviors.  
  *Context:* Describing server capabilities in a standardized way allows clients to dynamically adjust their operations, improves interoperability, and facilitates tooling or automation.  
  *Issues:* [#21](https://github.com/w3c/lws-ucs/issues/21)

### Storage and Resource Management

- <dfn>Storage Flexibility</dfn>
  **As a** user, **I want** the ability to dynamically split or aggregate storage units, **so that** I can adjust capacity and organization as my needs evolve.  
  *Context:* Flexible storage supports scalability and customization.  
  *Issues:* [#110](https://github.com/w3c/lws-ucs/issues/110), [#136](https://github.com/w3c/lws-ucs/issues/136), [#127](https://github.com/w3c/lws-ucs/issues/127), [#69](https://github.com/w3c/lws-ucs/issues/69), [#70](https://github.com/w3c/lws-ucs/issues/70)

- <dfn>Hypermedia Authoring</dfn>
  **As a** developer, **I want** consistent mechanisms for authoring hypermedia representations (e.g., JSON-LD, Siren), **so that** clients can navigate and interact with APIs uniformly.  
  *Context:* Standardized hypermedia improves API usability.  
  *Issues:* [#33](https://github.com/w3c/lws-ucs/issues/33), [#124](https://github.com/w3c/lws-ucs/issues/124)

---
