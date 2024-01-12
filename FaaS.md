# Fediverse as a Service
The vision for Fediverse as a Service is a decentralized and distributed Platform as a Service, Fediverse style.
The objective is to make expensive centralized corporate cloud providers like AWS obsolete.
Everyone *wants* to like serverless these days, but it's costly on AWS. Not so on FaaS.

### Requirements
* Resilient: No data should ever just dissapear unless requested. Distributed systems excel at this.
* Available: When a user requests data, it should be there. Distributed systems once again fit the bill.
* Fast: The user should not have to wait a long time to get their data. Tradeoffs required here.
* Scalable: The user experience should not change as the number of participating nodes increases.
* Cheap: Corporate cloud providers are charging market rates to make a profit. This project should instead be treated as community infrastructure.
* Secure: Sensitive data should only be knowable to the user and parties they trust.

### Architecture
Long term slow storage: Encryption and redundant sharding
Short term fast storage: Trusted local servers selected by the user that cache sensitive data and microservices via WASM containers; user's entrypoint to the FaaS system
