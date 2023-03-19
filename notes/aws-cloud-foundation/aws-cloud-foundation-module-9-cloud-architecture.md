# Everything fails, all the time

## Topics

- AWS Well-Architected Framework
- Reliability and high availability
- AWS Trusted Advisor

# Cloud architects

Cloud architects engage with decision makers to identify the business goal and the capabilities that need improvement. They ensure alignment between technology deliverables of a solution and the business goal.

# AWS Well-Architected Framework

AWS Well-Architected Framework is a guide that is designed to help you build the most secure high performing, resilient, and efficient infrastructure possible for your cloud applications and workloads.

It provides a set of foundational questions and the best practices that can help you evaluate and implement your cloud architectures.

# Oprational Excellence pillar

Oprational Excellence pillar focuses on the ability to run and monitor systems to deliver business value and to continually improve operations. Key topics include managing and automating changes, responding to events, and defining standards to successfully manage daily operations.

Six design principles for operational excellence in the cloud:
- Perform operations as code -> define your entire workload (that is applications and infrastructure) as code.
- Annotate documentation -> focus on automating the creation of annotated documentation after every build, annotation can be used as input to your operations as code.
- Make frequent, small, reversible changes -> design workloads to enable components to be updated regularly, make changes in small increments that can be reversed if they fail.
- Refine operations procedures frequently
- Anticipate failure
- Learn from all operational events and failures -> share what is learned across teams and throughout the entire organization.

# Security pillar

Security pillar focuses on the ability to protect information, systems, and assets while delivering business value through risk assessment and mitigation strategies. Security pillar focuses on the key areas of protecting confidentiality and integrity of data, identifying and managing who can do what or privilege management, protecting systems, and establishing controls to detect security events.

Seven design principles that can improve security:
- Implement a strong identity foundation -> implement the principle of least privilege and enforce separation of duties with appropriate authorization for each interaction with your AWS resources.
- Enable traceability -> monitor, alert, and audit actions and changes to your environment in real time. Integrate logs and metrics with systems to automatically respond and take action.
- Apply security at all layers -> apply defense-in-depth and apply security controls to all layers of your architecture.
- Automate security best practices -> automate security mechanisms to improve your ability to securely scale mroe rapidly and cost effectively.
- Protect data in transit and at rest -> classify your data into sensitivity levels and use mechanisms such as encryption, tokenization, and access control where appropriate.
- Keep people away from data -> reduce the risk of loss or modification of sensitive data due to human error, create mechanisms and tools to reduce or eliminate the need for direct access or manual processing of data.
- Prepare for security events -> incident management process that aligns with organizational requirements, run incident response simulations and use tools with automation to increase your speed of detection, investigation, and recovery.

# Reliability pillar

Reliability pillar focuses on the ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand and mitigate disruptions such as misconfigurations or transient network issues. Key topics include setup, cross-project requirements, recovery planning, and handling change.

Five design principles that can increase reliability:
- Test recovery procedures -> test how your systems fail and validate your recovery procedures.
- Automatically recover from failure -> monitor systems for key performance indicators and configure your systems to trigger an automated recovery when a threshold is breached.
- Scale horizontally to increase aggregate system availability -> replace one large resource with multiple smaller resource and distribute requests across these smaller resources to reduce the impact of a single point of failure on the overal system.
- Stop guessing capacity -> monitor demand and system usage and automate the addition or removal of resources to maintain the optimal level for satifying demand.
- Manage change in automation -> use automation to make changes to infrastructure and manage changes through automation.

# Performance Efficiency pillar

Performance Efficiency pillar focuses on the ability to use IT and computing resources efficiently to meet system requirements and to maintain that Efficiency as demands or technologies change. The key areas to review are: selecting the right resource types and sizes based on workload requirements, monitoring performance, and making informed decisions to maintain efficiency as business needs evolve.

Five design principles that can improve performance efficiency:
- Democratize advanced technologies
- Go global in minutes -> deploy systems in multiple AWS Regions to provide lower latency and a better customer experience at minimal cost.
- Use serverless architectures -> utilize serverless architectures to remove the operational burden of running and maintaining servers to carry out traditional compute activities.
- Experiment more often -> perform comparative testing of different types of instances, storage, or configuration.
- Have mechanical sympathy -> use the technology approach that aligns best to what you're trying to achieve.

# Cost Optimization pillar

Cost Optimization pillar focuses on the ability to run systems to deliver business value at the lowest price point. This pillar focuses on the areas of: understanding and controlling when money is being spent, selecting the most appropriate and right number of resource types, analyzing spending over time, and scaling to meet business needs without overspending.

Five design principles that can optimize costs:
- Adopt a consumption model -> pay only the computing resources that you require, increase or decrease usage depending on business requirements and not by using elaborate forecasting.
- Measure overall efficiency -> measure the business output of the workload and the costs that are associated with delivering it.
- Stop spending money on data center operations
- Analyze and attribute expenditure -> the cloud makes it easy to accurately identify system usage and costs, and attribute IT cost to individual workload owners.
- Use managed and application-level services to reduce cost of ownership -> reduce the operational burden of maintaining servers for tasks such as sending email or managing databases.

# Reliability and availability

## Reliability

Reliability is a measure of your system's ability to provide functionality when desired by your user.

Reliability is the probability that an entire system will function as intended for a specified period.

A common way to measure reliability is to use statistical measurements such as Mean Time Between Failures (known as MTBF).

MTBF is a total time in service over the number of failures.

## Availability

Availability is the percentage of time that a system is operating normally or correctly performing the operations of it or normal operation time over total time.

Availability is reduced any time the application isn't operating normally including both scheduled and unscheduled interruptions.

Availability is also defined as the percentage of uptime, that is length of time that a system is online between failures over a period of time (which is commonly one year).
