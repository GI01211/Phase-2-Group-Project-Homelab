Building a Multi-Subnet Cybersecurity Training Lab on AWS: All-AWS Security Services

Objective
This project challenges you to collaboratively build a multi-subnet cybersecurity training lab on AWS. Working in teams of six, you'll gain hands-on experience with securing cloud infrastructure using native AWS security services, network segmentation, and security best practices. This version replaces open-source tools with equivalent AWS security features and services.
e primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.


Learning Objectives:
Understand the benefits of using multiple subnets for security segmentation.
Collaborate effectively within a team to configure a secure cloud environment using AWS services.
Implement AWS security features like Security Groups and Network Access Control Lists (ACLs) to control network traffic flow.
Utilize AWS services like Amazon GuardDuty for threat detection, Amazon Inspector for vulnerability scanning, and Amazon CloudWatch for comprehensive monitoring.
Gain experience with AWS WAF (Web Application Firewall) for web application security.


Team Formation:
Instructors will create teams of six, ensuring a balance of skill sets and experiences.
Each team will elect a team lead to coordinate communication and task delegation.




Project Tasks:
Pre-Lab Review:
Review the guide outlining the lab components and configurations.
Research security best practices for cloud environments (e.g., shared responsibility model, least privilege).
Teams will create a shared repository (e.g., Git) to store research findings and any relevant articles.


VPC and Subnet Creation:
Teams will configure the VPC and subnets:
Create a VPC with a designated CIDR block.
Create four subnets with specific CIDR blocks for public access, training tools, Active Directory (optional), and optional Docker containers.
Team members will collaborate on configurations, ensuring shared understanding.
Document the VPC and subnet creation process with screenshots in the team repository.
Internet Gateway and Route Tables:
Teams will configure an internet gateway for the Public subnet and create route tables for each subnet:
Public subnet: Route to the internet gateway for internet access.
Other subnets: Configure routing as needed based on communication requirements.
Document the configuration process with screenshots in the team repository.
Security Group and Network Access Control List (ACL) Creation:
Each team will create dedicated Security Groups for each instance type (training tools, Windows Server).
Teams will collaborate to define Security Group rules and configure ACLs for subnets:
Allow necessary inbound and outbound traffic for each instance type.
Restrict traffic flow as needed for security (e.g., outbound traffic for specific training tools).
Use ACLs for additional granular control within subnets.
Document the security group and ACL creation process with screenshots and explanations in the team repository.




Launching Instances:
Teams will coordinate the launch of instances using appropriate AMIs and instance types:
Training tools (Kali Linux) in the Training subnet
Optional Windows Server instance (AD subnet)
Team members will take turns launching instances and configuring access using key pairs.
Document the instance launch process with screenshots in the team repository.
AWS Security Services Configuration:
Teams will configure AWS security services to enhance the lab environment:
Enable Amazon GuardDuty for threat detection within the VPC.
Use Amazon Inspector to scan launched instances for vulnerabilities.
Configure AWS WAF to protect any web applications deployed within the training environment.
Leverage Amazon CloudWatch for comprehensive monitoring:
Configure CloudWatch Logs to collect logs from launched instances for security analysis (replacement for SIEM functionality).
Set up CloudWatch metrics and alarms to monitor key security indicators (e.g., failed login attempts, network traffic anomalies) (replacement for IDS/IPS functionality).





Final Deliverables:
Repository: A shared repository containing all research materials, documentation of each configuration step, and screenshots.
Technical Documentation: A comprehensive document outlining the entire project, including downloads, installations, detailed configurations, and descriptions of the AWS security services used (replacements for tools and applications).
Professional Paper (1250 words):
Identify the various AWS security components used in the lab (Security Groups, ACLs, GuardDuty, Inspector, CloudWatch Logs, CloudWatch metrics/alarms, WAF).
Discuss how these services achieve the functionalities typically provided by SIEM, IDS/IPS, firewall, and monitoring tools in a traditional cybersecurity environment.
Networking Diagram: A visual representation of the network topology, including subnets, instances, and their connections.





Presentations:
Technical Audience: A detailed presentation for a technical audience, explaining the project's objectives, implementation details using AWS security services, and functionalities.
Non-Technical Audience: A simplified presentation for a non-technical audience, providing a high-level overview of the project's purpose, security concepts using AWS services, and benefits of the training lab.
Additional Notes:
Instructors will provide a detailed rubric with specific criteria for each deliverable.
Teams are encouraged to leverage AWS documentation and tutorials for specific security service configurations.
Remember, security is an ongoing process. Consider including recommendations for future enhancements using additional AWS security services in your reflection papers.
