# Center for Internet Security

| Start Date | End Date  |
| ---------- | --------- |
| June 2012  | Oct. 2021 |

## Titles Held

- Security Software Developer
- Technical Product Manager
- Technical Product Executive
- Software Architect

## Roles

- Individual Contributor
- Engineering Team Lead
- Product Owner
- Software Architect

## General Description
My experience at CIS has encompassed numerous facets of software development within the context of the industry-recognized security best practices contained in both CIS Benchmarks and the CIS Controls. I have grown from an individual developer focused on a single software product to software architect level, contributing to and integrating multiple software offerings. I have strived to focus on SecureSuite stakeholders, both internal and external; those organizations who have invested in the CIS non-profit mission. I have led small teams of developers, provided mentoring, career development, and training opportunities. I have acted as a product owner, guiding the vision of our software and helping to achieve that vision using agile software development methodologies. Because our teams have been small, it was necessary to assume multiple roles including member support, new member orientations, and security automation content development.

My software development experience has focused on Groovy, Java, Python, and C#. I have experience
with application frameworks such as Grails, Micronaut, and Spring; build tools such as Gradle and Ant; and cloud services in AWS such as API Gateway, Lambda, DynamoDB, SNS, SQS and the cloud
development kit (CDK). In my most recent role as Software Architect, I have performed as both high-level designer of multiple software products as well as a "solver"; a subject-matter expert utilized by teams to solve the most technical issues. Within these two facets, I've gained both design/integration experience and have been able to contribute code to production systems.

## Software Architecture / Cooperative Ecosystem
In order to achieve the vision of "speeding policy to implementation", my role as Software Architect has encompassed an overarching theme of enabling security program orchestration, allowing the resources available to CIS SecureSuite members to interact in a standardized, automated and programmatically oriented manner. This "cooperative ecosystem" describes numerous integration services designed to define and implement the interactions between those resources.

- Work with each of the product engineering (PE) teams and their respective product owners to define
required interactions with their tooling.
- Actively engage with standards development organizations (SDOs) on defining requirements,
workflows and interactions.
- Utilize the resources within those SDOs, such as hackathons, workshops, and ongoing working group
meetings to prove the architectural ideas with running code, and to gain consensus with technical
peers.
- Continue to evangelize the needs for involvement in these activities internally, allowing for dedicated resources to create and maintain this ecosystem.
- Ongoing development and operational deployment of services specific to each set of tooling in order to put the design into production.

### Software Development
Proofs of concept, prototyping, and production code contribution were also part of my role as Software Architect.  As a subject matter expert within CIS' domain of security automation content creation and assessment, many projects required my assistance with either technical design, problem solving, or mentoring. Within the role, I was also able to develop the integration components which were ultimately utilized across engineering teams/products.

#### Data Exchange Layer
Utilizing the McAfee OpenDXL framework, I developed multiple services and publish/subscribe capabilities allowing for common functionality and interaction between products.

- New member onboarding services automated connectivity to the integration layer and generation of member license keys.
- License generation, verification, and revocation services allowed all CIS SecureSuite software tools to verify the validity of member license keys.
- Industry average services allowed members using specific software tools to anonymously contribute self-assessment results to overall industry averages, as well as to continuously receive updates to data via subscription.

### Standards Development Organizations

- Internet Engineering Task Force (IETF); Security Automation & Continuous Monitoring working group
- Open Vulnerability and Assessment Language (OVAL) contributor, area supervisor and board member
- Security Content Automation Protocol (SCAP) implementer, contributor, and working group member


## CIS Configuration Assessment Tool (CIS-CAT)
Written in Groovy, CIS-CAT Pro Assessor (a.k.a. CIS-CAT) is the flagship tool offered in CIS SecureSuite membership. CIS-CAT provides automated posture attribute collection and evalution against recommendations made by CIS Benchmarks. With support for nearly 100 Benchmarks, CIS-CAT is
architected as a library/component-based application, allowing for multiple deployment models, such as a command-line, graphical, or ReST-base web interface.

- Expanded CIS-CAT capabilities to support standardized content using the Security Content Automation Protocol (SCAP), culminating in the tool's validation against verion 1.2 of the SCAP specification.
- Added more than 130 system characteristic collection "probes", used to acquire security-relevant posture attributes from target systems under assessment.
- Simultaneously refactored entire Java-based application to Groovy in order to modularize the software architecture and enable remote endpoint assessment capability; all while maintaining and enhancing the existing application per member needs and product roadmap.
- Enabled remote endpoint posture collection and assessment using SSH and WinRM for Unix/Linux/Mac and Windows operating systems, respectively.
- Acted as the CIS-CAT Product Owner, continued to manage the roadmap, prioritizing tasks based on
member feedback, developer capacity, and proposed functionality.
- Included support for the Script Check Engine (SCE), the specifications for which were developed for the OpenSCAP project (Red Hat). Implemented support for execution of Windows batch scripts,
PowerShell and VBScript, along with shell scripts in Unix/Linux environments.
- Added numerous reporting features including evidence-enabled HTML reports, JSON, CSV, and plain-text outputs.

## Optimus Content Transformation System
The Optimus project is designed to export configuration recommendations from the CIS WorkBench application (the community portal in which CIS benchmarks are developed and tailored) into standards-based security automation content, which can be used with the CIS-CAT Pro Assessor application.  Optimus is a completely serverless application deployed to AWS using cloud formation stacks maintained using the AWS Cloud Development Kit (CDK).

- Designed the framework of the Optimus application to utilize AWS infrastructure.
- Developed and deployed cloud formation stacks using AWS Cloud Development Kit (CDK) to include creation of IAM roles and policies, S3 buckets, DynamoDB tables, Lambda functions, Layers, and CodeBuild projects.
- Development of transformation functions, deployed as Lambda functions, using Groovy.
- Migration of legacy Ruby transform code to Groovy and fitting into the new export format.
- Enabled the application to handle future enhancements including vendor content generation, remediation content generation, or other automation formats.

### SecureSuite API
Developed in conjunction with the Optimus project, the SecureSuite API are publicly exposed ReST endpoint, deployed via AWS API Gateway. The API offers both members and non-members programmatic access to various SecureSuite resources such as CIS Benchmark content available in multiple serializations (XML, YAML, or JSON), as well as CIS-CAT downloads. Authentication and authorization to SecureSuite member-only content is enabled through license key verification, and backend services utilize AWS Lambda functions and AWS Athena.

- Developed authentication using SecureSuite license verification via Lambda functions
- Enabled authorization to member-only resources via tokens and API Gateway Lambda Authorizers
- Contributed Groovy code for various API backend functions such as CIS-CAT downloads and access to various serializations of CIS Benchmark content.

## CIS Controls Self-Assessment Tool (CSAT)
The CIS Controls Self-Assessment Tool (CSAT) allows members, using a web-based user interface, to assess and track over time, their organizational maturity when implementing the CIS Controls.  The CIS Controls represent a prioritized set of actions designed to protect an organization from known cyber-attack vectors.  The CSAT application allows member organizations to create assessments, measuring the effectiveness of control and sub-control implementation.

From the technical perspective, the CSAT application is built using the Grails application framework, persisting data to a Neo4j graph database, allowing for easy visualizations of the relationships between data entities.  The CSAT application also integrates with the CIS cooperative ecosystem of resources using OpenDXL, allowing for membership key verification, as well as the participation in industry average services and calculations.

- Overall architectural design including technology decision-making, data model design, application and integration frameworks required to support a member-hosted version of CSAT.
- Implementation of all integration functions with CIS-hosted version of CSAT, supporting a microservices-like model, to include service clients, service request handlers, and publish/subscribe functions.
- Provided assistance to the team on all technical implementation issues, including high-level data modeling and relationship design, as well as acting as a developer on the team, implementing microservices and all cooperative ecosystem interactions.

## Operational Support & Stakeholder Engagement
Prior to the establishment of a dedicated operations team, I was responsible for all CIS-CAT related support request resolution, including member requests, non-member questions, XML customizations, and bug fixes.

- Responsible for CIS-CAT release procedures including source control, documentation, script updates, compiling, packaging and deployment to CIS WorkBench.
- Facilitated “New Member” Orientations, beginning with individual member orientations and moving to group orientations as the number of members increased from 300 to their current levels (2000+).
- Prospect demos with the outreach team and technical support for CIS-CAT trials.

