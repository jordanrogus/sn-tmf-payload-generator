# sn-tmf-payload-generator

The implementation of SN Telco products that utilize TMF APIs may face delays due to the requirement of setting up and configuring upstream systems (i.e., CPQs) to send TMF-compliant payloads for initiating SN processes. In practice, SN development teams often spend significant amounts of time creating mock payloads that adhere to TMF specifications, allowing them to begin SN development. However, the TMF Mock Payload Generator utility simplifies this process, facilitating faster delivery and the ability to provide development teams with a greater amount of test data in a shorter timeframe. Furthermore, this utility supports bulk submission of TMF APIs, enabling efficient performance testing.

Version History
- v1.0.0 - July 2023 - Initial release with TMF622 POST compatability

Features
1.	TMF622 (Product Order) POST compatibility for generating mock payloads from a ServiceNow modelled Product Offering using no-code interfaces.
2.	Ability to reference records in the system, such as core data (e.g., account and product offerings), for generating instance-specific payloads.
3.	Intelligent setup where templated records are automatically created (per API), enabling users to conveniently fill in the desired data (e.g., account or contact) without additional manual steps.
4.	Customizability, allowing users to fill out predefined OOTB SN TMF API parameters to influence how the payload is sent into ServiceNow (e.g., synchronous, or asynchronous).
5.	Ability to store a library of mock payloads within ServiceNow for easy access and management.
6.	Streamlined payload generation through the ability to copy entire payload hierarchies or specific orderable items and their associated records. This simplifies the process of creating or modifying payload generation records.
7.	Functionality to send the payload to the SN instance via REST APIs, allowing testing against out-of-the-box (OOTB) APIs. Users will be able to view information on created records or detailed error messages generated from the APIs.
8.	Performance testing capability that enables programmatically submitting N number of API calls to the instance.

SN Application Dependencies
1.	Product Catalog Management Core (v6.0.0)
2.	Product Inventory Advanced (v3.0.0)
3.	Customer Service (v23.8.2)
4.	Order Management for Telecom, Media & Tech (v4.0.0)

Usage Notes
1. Review and update application properties (TMF Mock Payload Generator > Administration > Properties)
