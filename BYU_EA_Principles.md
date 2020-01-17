# BYU Enterprise Architecture Principles

BYU's Enterprise Architecture framework consists of four distinct architecture types:

-   Business Architecture

-   Information Architecture

-   Application Architecture

-   Platform Architecture

Business Architecture documents and models an organization's policies, processes, work activities, artifacts, and assets. Specifically, Business Architecture answers the following questions concerning BYU's organizations and processes:

-   What do they do?

-   Who does it?

-   Why do they do it?

-   How do they do it?

-   When do they do it?

-   Where do they do it?

Information Architecture documents and models key information assets, the applications that use them to enable business processes, and how applications and information together support the enterprise's functions. The information architecture also specifies which parts of the business process are supported by each application and where each type of data is stored and managed.

**Application Architecture** principles document how applications are designed, built, and integrated. The application architecture conforms to the business domains that enable and support the execution of BYU's business processes.

Platform Architecture consists of the combination of software, middleware, hardware infrastructure and development frameworks that enable the development, deployment, operation, integration and management of applications.

BYU's Enterprise Architecture principles are founded on the ideas of domain-driven design (DDD). If you're not familiar with DDD, the book *Domain-Driven Design Distilled* by Vaughn Vernon is a short, easy-to-understand description.

A glossary is included at the end of this document.

## What are Principles?

Principles are simple statements of values that inform and support the way an organization fulfills its mission. Enterprise architecture principles are intended to guide IT decision-making processes, serving as a base for IT architectures, development policies, and standards.

A common misunderstanding concerns the difference between principles and standards. While they are similar in nature, principles and standards differ significantly in intention and application. Essentially, principles provide high-level guidance on *what* should happen within architecture, while standards define *how* they should happen. For example, a standard may state something like: "*All web pages must be WCAG 2.0 compliant."* While a principle would give higher level guidance such as: *"All data, information, applications and processes must be easy to use and must be accessible to all relevant parties."*

The remainder of this document describes the overarching Enterprise Architecture principles followed by principles for each of the architecture types (Business, Information, Application, and Platform) and the domains within those architecture types.

## Overarching Enterprise Architecture Principles 


### Principle 1: Broadly Applicable


**Statement**: BYU's Enterprise Architecture applies to any information technology system across the University regardless of who pays for and builds it.

**Rationale**: A consistent framework for information technology promotes better, more interoperable solutions.

**Implications**: 

-   This applies to all BYU systems, data and infrastructure.

-   University-wide, mission critical solutions will be subject to enterprise architecture review[^1] and, where deemed appropriate, require ITPC approval.

### Principle 2: Technology Provides Business Value

**Statement**: Business value is created when business unit and IT professionals work together.

**Rationale**: Information Technology has the most value when business and IT professionals work together to align solutions with BYU's strategic plans, and other university-level direction, concepts, and objectives.

**Implications**:

-   IT is not merely a contractor delivering whatever the business unit customer asks for, but a partner in creating value for the business and meeting strategic goals.

-   Business and IT professionals work together to determine how to solve business problems with IT.

-   Architectures will be generated with a specific purpose and for a specific audience to ensure they meet the expectations and needs of its intended stakeholders.

### Principle 3: Holistic User Experience

**Statement**: People and organizations who have relationships with the University should use systems that are consistent, cohesive, and comprehensive.

**Rationale**: A holistic user experience facilitates and streamlines the primary activities of the user while reducing errors, increasing user satisfaction, and protecting people from security and privacy breeches.

**Implications**:

-   Users deserve experiences that are comprehensive and complete, meaning that the entire interaction can happen without shifting between different contexts and applications.

-   Consistent user experiences insulate people from the proliferation of services implied by respecting business contexts.

-   User experience is not the same thing as user interface

-   User access to services should be mediated by web and mobile applications that operate in similar ways

-   Services, not user interfaces, are responsible for workflow.

-   Services will be available to people through multiple customer-facing applications, mediated via an API.

### Principle 4: Support Channel and Device Neutrality 

**Statement**: We do not control the access devices students, faculty, and staff use and so applications must work flexibly across multiple devices and in parallel channels.

**Rationale**: BYU is a "Bring Your Own Device" environment and supporting multiple platforms provides the best user experience.

**Implications**:

-   Most students are "mobile first" and our applications must be as well.

-   Separating presentation (UI) from the business logic delivered via API ensures consistent experience and outcomes even on different devices.

### Principle 5: Independently Deployable, Reusable Components 

**Statement**: BYU's Enterprise Architecture will be built on reusable, loosely coupled, modular components that can be independently deployed.

**Rationale**: Independently deployable, reusable components provide opportunities to reduce IT development costs and time by reducing development complexity and leveraging investments in existing systems. Modular components improve system ability to adapt to changing requirements.

***Implications***:

-   Data will only be shared between components using well-defined contracts, not shared databases.

-   Loosely coupled modular components must exist in a source code repository, be documented, and be searchable for ongoing support and future use.   

-   APIs will be used wherever possible to ensure multiple applications can take advantage of business workflow.  

-   IT organizations across the university should make use of open-source code whenever possible.

-   IT organizations across the university should provide their code to others inside and outside the university through sharable code repositories.

### Principle 6: Leverage Investments 

**Statement**: All systems will leverage existing and planned components, enterprise software, management systems, infrastructure and standards.

**Rationale**: BYU has invested heavily in a number of processes, technologies, infrastructures, and standards. Therefore, to maximize BYU's return on investment, all proposed systems should leverage existing systems as much as possible.  

**Implications**:

-   Considering how to leverage or reuse investments is applicable to all technology domains.

-   Advocates of proposed solutions should first determine how they might be completed using existing services, modules, or systems. 

-   Searchable repositories and a commitment to populate them are needed for this to be possible.

### Principle 7: University Systems are Secure 

**Statement**: Information security protects the University, information systems, people, and data.

**Rationale**: The University, students, faculty, staff, alumni, and partners can all be harmed by poor security practices.

**Implications**:

-   Systems and applications are instrumented with security monitoring and alerting

-   Systems and applications are patched regularly to avoid known exploits.

-   A well-documented inventory of systems and software is maintained as an aid to securing *all* University IT systems.

-   Information security systems are automated to the extent possible to ensure they can be scaled to cover all University IT systems.

-   Education, training, and awareness are a critical component of IT security to ensure the people developing and using IT systems are partners in keeping them secure.

### Principle 8: Balance Access and Security 

**Statement**: System designs, standards, and practices should make university information available to appropriate audiences while protecting information the university controls in accordance with legal, contractual, and ethical requirements.

**Rationale**: Information is a vital institutional resource whose value is enhanced when used appropriately and diminished when misused, misinterpreted, or when access is unnecessarily restricted.  

**Implications**:

-   While providing access to and safeguarding the integrity of University information is a shared university responsibility, information stewards[^2] are responsible for classifying the information in their units and for the processes that generate, distribute, share, and/or receive university information.

-   Decisions about providing access to information are based on the classification and the value of the assets, which is determined by its use, sensitivity, and importance to the university and in compliance with university policy, state and federal regulations, and other obligations regarding privacy and confidentiality of information.

### Principle 9: Protect Privacy 

**Statement**: We build systems that protect people and allow them choice and autonomy about data that is about them.

**Rationale**: Good privacy practices protect people and the University from harm.

**Implications**:

-   Be clear about what data is being collected and why.

-   Ensure data collection and storage is based on legitimate business interests.

-   University-held data is reviewed regularly to ensure it needs to be retained based on legitimate business interests. Once the business interest has passed the data is retired and removed from University systems.

-   Ensure that people consent to uses of their data, where appropriate.

-   Make it easy for people to review, modify, and delete the data about them where appropriate.

-   Create secure systems that protect data.

-   Never sell or trade personal data with third parties. Data is only shared with third parties for legitimate University business purposes.


## Business Architecture Principles

Business architecture is a part of enterprise architecture that aligns strategic objectives by developing common understanding about the organization's strategy, constituents, units, products and services, assets, and processes. It does this by creating models and common vocabulary.

BYU's Business Architecture Principles are founded on the idea that IT and University business units collectively represent the University to people and organizations who have relationships with the University (e.g. students, faculty, staff, and alumni).

The principles of business architecture guide those developing technology solutions.

### BA Principle 1: BA is about the business -- not IT. 

**Statement**: Business architecture is not constrained by technology.

**Rationale**: Business architecture describes the business model independent of its supporting technology and provides the foundation for the analysis of opportunities for automation.

**Implications**:

-   Eliminate technology constraints when defining business architecture and ensure processes are described at the business process level for analysis and design.

-   University units and IT organizations must have a common vision of both a unit's business functions and the role of technology in them.

-   The university unit and IT have **joint responsibility** for defining the IT needs and ensuring that the solutions delivered by the development teams meet expectations and provide the projected benefits.

-   Business owners participate in IT decisions as part of a domain team to determine the best choices for business architectures.

### BA Principle 2: BA is about Defining, Optimizing, and Maintaining Business Models 

**Statement**: Business models comprise the processes (workflows) and data structures the business domain uses to conduct their work. These models must be documented, analyzed, and understood before they can be automated.

**Rationale**: Focusing on business models aligns design with the needs of the business domain and increases opportunities for increasing efficiency and correctness of eventual IT solutions.**

**Implications**:

-   Analyze business models to simplify, integrate, eliminate redundancy, and increase efficiency.

-   Models are domain specific. There may be sub domains with different models.

### BA Principle 3: Enterprise Business Design is Balanced with Architectural Realities 

**Statement**: The business models of the University and the architectures that serve them are balanced to recognize the realities of IT systems and the cost of the system to the University.

**Rationale**: Models and architectures are aligned to serve the business and ensure that solutions can be efficiently implemented and maintained.**

**Implications**:

-   The architecting, designing, and building of solutions must be considered within the context of the enterprise's business processes, policies, and desirable practices.

-   Since solving business problems often involve buying rather than building solutions, the realities of the purchased systems must be taken into account and domain models modified where such modification makes implementation and operation less expensive without undue changes to the needs of the business.

-   The flexibility and degrees of freedom in domain model design is proportional to the degree to which the business domain is core (strategic and differentiating) to the University's mission (as opposed to being supporting or general infrastructure).

### BA Principle 4: BA Evolves as Business Needs Change 

**Statement**: Business architecture is an intentional model of the business processes of the University that supports and facilitates the use of technology in the business. BA provides a foundation for future analysis, effort, and decision-making.

**Rationale:** BA is not a one-time analysis of a business environment but an ongoing need as the business grows and evolves.

**Implications:**

-   Domain teams that include both business and IT experts are responsible for creating the business architecture for their respective domains. Domain teams meet as needed but exist so long as the business domain does.

-   Domain teams should identify opportunities for common services and implement them in such a way that there is an opportunity for collaboration with another department, program, or unit of the university.

-   Use the existing business architecture description and deliverables as a starting point for future efforts, unless an organization has fundamentally changed.


## Information Architecture Principles 

Information and Data Architecture documents and models key information assets, the applications that use them to enable business processes, and how applications and information together support the enterprises functions. The information architecture also specifies which parts of the business process are supported by each application and where each type of data is stored and managed.

### IA Principle 1: Information is an Asset 

**Statement**: Information is an asset that has value to the enterprise and needs to be managed and treated much like a physical asset.

**Rationale**: Information is a valuable corporate resource; it has real, measurable value. Information is used to aid decision-making and accurate and timely information is critical to accurate and timely decisions.

**Implications**:

-   We must carefully manage information to ensure that we know where it is, can rely on its accuracy, and can obtain it when and where we need it. An information asset's classification is determined by its value and risk. A fundamental understanding of the value of an information asset to the business and the business risk if it is exposed, corrupted, or lost is essential to determining the appropriate strategies and investments to make for protecting and managing it.

-   Ensure that all organizations understand the relationship between the value of information, sharing of information, and accessibility to information.

-   Make the cultural transition from "information ownership" thinking to "information stewardship" thinking.

-   Measure and document the current value, risk, and cost of the asset as you would any physical enterprise asset, such as property or equipment.

-   Make information accessible to its authorized end users in an easy, seamless manner.

### IA Principle 2: Each Business Domain is Responsible for its Own Information Architecture 

**Statement**: Information is defined by the domain it lives in. Different business contexts will have responsibility for specific information relevant to their domain.

**Rationale**: The nature of data makes it impossible to create consistent definitions across different contexts. An "order" in one context may contain different fields and have different impacts than an "order" in another. Independence in defining the meaning of data in different contexts aids flexibility and agility. Flexible, agile responses to changing business needs requires that each business domain be responsible for the information it needs to carry out its mission.

**Implications**:

-   Each business domain is responsible for defining the meaning of information within their context.

-   Each domain must ensure that its data model is protected from unnecessary dependence on other domain models or decide to conform to the other domain's definitions.

-   The University API represents a universal interchange language that domains can use to exchange information.

-   Some information will be duplicated across the enterprise.

-   Business domains must protect their data from corruption by other data in other business domains.

-   Each domain must take steps to ensure it has the correct information and that it matches their domain model.

### IA Principle 3: Information is Accessible and Shared 

**Statement**: Information is appropriately shared across enterprise functions and organizations.

**Rationale**: Students, faculty and staff must have access to the information necessary to perform their duties.

**Implications**:

-   University functions require access to the information necessary to make good decisions in a timely manner.

-   Information isn't owned by any specific individual, role, or group, but rather is available as necessary to accomplish University goals.

-   All university information has a steward who determines the appropriate access control to protect the information from inappropriate sharing.

-   University faculty, staff, and students have access to information necessary to perform their work.

-   Personal information is shared by and through users wherever possible, especially when that information must be shared with third parties.

### IA Principle 4: Information Stewards Manage Access Policy 

**Statement**: The primary responsibility of an information steward is to establish reasonable policies for the information in their stewardship that balances access with protecting University assets.

**Rationale**: Policy is broadly applicable and reusable. Furthermore, policy can be automatically applied in most cases, expediting access.

**Implications**:

-   The vast majority of data access requests will be automatically handled by attribute-based access control (ABAC) at the service interface.

-   Exceptions to access policies (i.e. negotiated data sharing agreements) are limited to a small set of edge cases and single-use applications.

-   Policy statements should be human readable and translatable to direct machine mediate wherever possible.

-   Policies about access should be open and public.

-   Access policies should follow a policy life cycle.

### IA Principle 5: Information Stewards are Accountable 

**Statement**: Information stewards are formally assigned accountability for establishing and enforcing the information policies that govern the access, security, quality, and classification of information assets within their domain of responsibility.

**Rationale**: One of the benefits of an architected environment is the ability to share information (e.g., text, video, sound, etc.) across the enterprise. As the degree of information sharing grows and business units rely upon common information, it becomes essential that policies and decisions about information within their stewardship are made by the information steward.

**Implications**:

-   Real stewardship dissolves the information \"ownership\" issues and allows the information to be available to meet all users\' needs. This implies that a cultural change from information \"ownership\" to information \"stewardship\" may be required.

-   Stewards manage the information assets on behalf of others and in the best interests of the organization.

-   Stewards must have the authority and means to manage the information for which they are accountable and be responsible for meeting quality requirements levied upon the information for which the trustee is accountable.

## Application Architecture Principles 

Applications and Systems Architecture represents the models for how applications are integrated and identifies the business systems that enable and support the execution of BYU's business processes. 

### AA Principle 1: Applications Conform with Domain Models 

**Statement**: Applications, whether custom or purchased, are the product of and influenced by a domain model created by a cross-functional domain team.

**Rationale**: Both technical and business interests should be represented when making decisions to create effective and flexible solutions.

**Implications**:

-   Domain-driven design will be used to architect and build applications that align with business needs.

-   Architectural design precedes application design and development.

### AA Principle 2: Each Domain Model Represents an Independent Business Context 

**Statement**: Independent contexts are bounded to preserve independence

**Rationale**: Bounded contexts provide a way of managing complexity in large applications by breaking them into separate conceptual modules.

**Implications**:

-   Each bounded context is free to choose its own names for concepts within it and should have exclusive access to its own persistence store.

-   Applications do not share databases.

-   Bounded contexts map closely to components.

-   The model for a bounded context must be internally self-consistent but is independent of other models in other contexts.

-   Each bounded context is implemented in and accessed through an API-mediated service. Communication between contexts occurs through these APIs.

### AA Principle 3: Components Implementing a Bounded Business Context Communicate via Published Public Interfaces and Contracts 

**Statement**: Components do not share data except through APIs.

**Rationale**: APIs provide the means for independent domains to communicate and cooperate.

**Implications**:

-   Components are self-contained and built for a specific business context.

-   Components do not share data through a shared database.

-   Public interfaces might be RESTful, event-driven, message-based, or credential or claim-based APIs depending on the needs of the component.

-   Components must make efforts to protect the consistency of their internal data model from other components.

-   While components talk component-to-component where needed, use of an interchange language such as the University API is preferred for increased flexibility and understandability.

### AA Principle 4: Purchased and Open-Source Solutions are Preferred to Custom Solutions 

**Statement**: A decision to build custom applications should be made only after an analysis that considers other BYU sources and third-party alternatives.

**Rationale**: Decisions that are made without considering the alternatives may be expensive and difficult to support. There is no reason to re-invent something that already exists.

**Implications**:

-   Project teams, architects and system engineers will consider existing technologies before developing new ones.

-   An analysis of industry-leading third-party solutions will also be considered.

-   Consider "subscription" over purchasing where possible and practical.

-   Total Cost of Ownership should be a part of any analysis.

-   The decision to buy or build should take into account whether the context is core to the University mission, supports the University mission, or is generic. Core contexts are more likely to have unique business value and benefit from custom solutions.

### AA Principle 5: Applications are Built to Support Continuous Integration/Continuous Delivery Methods 

**Statement**: Continuous delivery supports getting new features, configuration changes, bug fixes, and experiments into production, or into the hands of users, safely and quickly and in a sustainable way.

**Rationale**: Deployments should be routine and predictable to reduce risk, lower costs, and increase speed to market.

**Implications**:

-   We will buy, develop, and use tools to support the deployment of systems, configurations, and bug fixes.

-   All code will have integrated tests.

-   Monitoring systems will detect failures and automatically roll back deployments when necessary.

-   There are no limited change windows for University IT systems. This does not imply that a product or domain team may not decide to limit changes for business reasons.

## Platform Architecture Principles 

### PA 1: Cloud-based Platforms are Preferred 

**Statement**: All new development will be cloud native to limit undifferentiated effort.

**Rationale**: On-premise solutions are more expensive to host and maintain. Cloud-based platforms have better overall security and feature sets that BYU can supply itself for the same cost.

**Implications**:

-   Cloud-based solutions should be picked when a choice is available.

-   The platform team's efforts will be best used in managing the cloud-based systems.

-   A managed access strategy is required to ensure security and control costs.

-   We will use a single public cloud partner. Use of alternatives must be approved by the CIO's office.

-   The use of cloud-native features is encouraged to leverage efficiencies of scale.

### PA 2: Enterprise Platforms are Available thru Self-Service 

**Statement:** The campus community can acquire enterprise platforms via an online order fulfillment process.

**Rationale:** The process to deploy approved university systems onto these platforms should be well-documented and simple to use.

**Implications:**

-   Members of the campus community can obtain enterprise platforms without a formal project.

-   Platforms are well documented, well supported and available to be used much like other platforms in industry.

-   Access control strategies should allow developers to easily get access to the platform resources they need. Access control strategies should minimize university expense.

### PA 3: Platforms are Monitored 

**Statement**: Our underlying platforms are monitored so that we know how they're being used, what the costs are, and can respond to threats quickly.

**Rationale**: Poorly monitored platforms can quickly get out of control, costing the University money or opening it up to security and privacy breeches.

**Implications**:

-   Each platform has a team assigned to monitoring it. This team is responsible for ensuring it happens.

-   Meaningful reports are created, and management regularly reviews them.

## Glossary 

The following is a brief glossary of terms used in the Enterprise Architecture Principles.

**API** -- Application Programming Interface. While the use of the term API is most often associated with REST based APIs, in this document it refers to any programmatic interaction between entities that is contract based and discoverable. Events, claims, and other related technologies are all considered APIs.

**Application** -- Application can refer to a back-end service, a mobile app, or a web application depending on the context.

**Bounded context** -- A logical boundary between services or applications corresponding to the business process of a particular domain or sub-domain that the service is built to model.

**Cloud-native** \-- Cloud-native applications are developed using technologies that package services in containers, deploy them idependently, and manage them on elastic infrastructure using agile DevOps methodologies and continuous delivery.

**Component** -- An independently deployable, self-contained module or service modeled around a business domain or sub-domain.

**Domain** -- the entities, behaviors, data, and processes for a particular business function of the university.

**Platform** -- the software, middleware, hardware infrastructure and development frameworks that enable the development, deployment, operation, integration and management of applications.

**Sub-domain** -- domains can be decomposed where required into sub-domains to ease modeling and increase comprehension. Sub-domains might be classified as "core" for those that are central to the university's mission, "supporting" for those that provide ancillary functions, or "generic" for those that are done by most businesses everywhere. A generic domain is not unimportant, just not unique.

## Meta

Version: 20191226  
Approved: January 17, 2020  by  
J. Kelly Flanagan  
CIO/VP Information Technology  


[^1]: *An enterprise architecture review is NOT an audit*. Rather, the purpose of the review is to help the project team leverage the existing architecture and common services, proactively identify the risks to a project, understand the university-wide context in which the proposed solution is to operate, and provide input on how BYU's architecture may need to be modified.

[^2]: See Information Governance procedures for descriptions of the roles and responsibilities of information stewards.
