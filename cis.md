# Center for Internet Security

| Start Date | End Date  |
| ---------- | --------- |
| June 2012  | Oct. 2021 |

## Titles Held

- Security Software Developer
- Technical Product Manager
- Technical Product Executive
- Software Architect

## General Description
My experience at CIS has encompassed numerous facets of software development within the context of the industry-recognized security best practices contained in both CIS Benchmarks and the CIS Controls. I have grown from an individual developer focused on a single software product to software architect level, contributing to and integrating multiple software offerings. I have strived to focus on SecureSuite stakeholders, both internal and external; those organizations who have invested in the CIS non-profit mission. I have led small teams of developers, provided mentoring, career development, and training opportunities. I have acted as a product owner, guiding the vision of our software and helping to achieve that vision using agile software development methodologies. Because our teams have been small, it was necessary to assume multiple roles including member support, new member orientations, and security automation content development.

My software development experience has focused on Groovy, Java, Python, and C#. I have experience
with application frameworks such as Grails, Micronaut, and Spring; build tools such as Gradle and Ant; and cloud services in AWS such as API Gateway, Lambda, DynamoDB, SNS, SQS and the cloud
development kit (CDK). In my most recent role as Software Architect, I have performed as both high-level designer of multiple software products as well as a "solver"; a subject-matter expert utilized by teams to solve the most technical issues. Within these two facets, I've gained both design/integration experience and have been able to contribute code to production systems.

## Project Work
TODO

### Software Architecture / Cooperative Ecosystem
In order to achieve the vision of "speeding policy to implementation", my role as Software Architect has encompassed an overarching theme of enabling security program orchestration, allowing the resources available to CIS SecureSuite members to interact in a standardized, automated and programmatically oriented manner. This "cooperative ecosystem" describes numerous integration services designed to define and implement the interactions between those resources.

- Work with each of the product engineering (PE) teams and their respective product owners to define
required interactions with their tooling.
- Actively engage with standards development organizations (SDOs) on defining requirements,
workflows and interactions.
- Utilize the resources within those SDOs, such as hackathons, workshops, and ongoing working group
meetings to prove the architectural ideas with running code, and to gain consensus with technical
peers.
- Continue to evangelize the needs for involvement in these activities internally, allowing for dedicated
resources to create and maintain this ecosystem.
- Ongoing development and operational deployment of services specific to each set of tooling in order to put the design into production.

#### Standards Development Organizations
IETF SACM
OCA
SCAP/OVAL/XCCDF
etc.

### CIS Configuration Assessment Tool (CIS-CAT)
TODO

### CIS Controls Self-Assessment Tool (CSAT)
TODO

### Optimus Content Transformation System
TODO

### SecureSuite API
TODO

## RAW


Software Architecture


CIS Configuration Assessment Tool (CIS-CAT Pro Assessor)
Written in Groovy, CIS-CAT Pro Assessor (a.k.a. CIS-CAT) is the flagship tool offered in CIS SecureSuite
membership. CIS-CAT provides automated posture attribute collection and evalution against
recommendations made by CIS Benchmarks. With support for nearly 100 Benchmarks, CIS-CAT is
architected as a library/component-based application, allowing for multiple deployment models, such as a
command-line, graphical, or REST-base web interface.

- Acted as the CIS-CAT Product Owner, continued to manage the roadmap, prioritizing tasks based on
member feedback, developer capacity, and proposed functionality.
- CIS-CAT Pro Assessor utilizes SSH to remotely collect/evaluate system state for Unix, Linux, and Apple
OSX operating systems, along with WinRM for Microsoft Windows operating systems.
- More than 130 "probes" have been implemented to enable the collection of security-relevant posture
attibutes.
- Included support for the Script Check Engine (SCE), the specifications for which were developed for the OpenSCAP project (Red Hat). Implemented support for execution of Windows batch scripts,
PowerShell and VBScript, along with shell scripts in Unix/Linux environments.

