# Data-Governance

Data is one of the most importanat resources an organization possesses in todays economy.

# WHAT IS DATA GOVERNANCE

* Data governance is a set of rules and procedures to manage an organization's data. It ensures data is accurate, secure, and usable for various purposes.
* Similar to how governments create laws, organizations set data policies to define how data is used, accessed, and protected.
* These policies cover data quality, data attributes, data access permissions, data security, regulations compliance, and data privacy.
* Organizations also implement controls (procedures and technology) to enforce these data governance standards.
* Successful data governance requires strong support from executives across the organization, not just the IT department.

# Data Governance Roles

* Data Stewardship: Overseeing data quality, security, privacy, and regulation compliance.
Organizational Data Steward: Leads data governance activities and connects technical and non-technical teams.
Works with Data Owners (senior leaders responsible for specific data areas) to define policies.
May delegate tasks to Subject Area Data Stewards (understand nuances of their specific data domain)

* Data Owners: Senior leaders responsible for a specific data domain (e.g., finance, HR).

* Data Custodians: (Often IT staff) implement technical controls to enforce data governance policies (e.g., configuring access controls).

# Collaboration is Key

The organizational data steward works with all these roles to ensure proper data governance:

* Vertically (across different levels) with data owners and subject area data stewards.
* Horizontally with data custodians responsible for implementing technical controls.
  
# Data Access Requirements

* Access to data is granted based on specific needs.
* Access level varies by data domain and can be limited to specific data fields.
* Example: Managers need access to employee names, contact info, and performance data, but not Social Security numbers.

# organizational example 

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/9b1f47c7-5ea0-46d6-9aa5-6678530fb286)

# Determining access requirements
it is essential to develop a data classification matrix. A data classification matrix defines categories, and disclosure implications for data.

# Table showing ana example of data classification.
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/555f37f7-455d-4f74-bf15-46e7c17be782)

# Access Permissions

It is granting access based on roles simplifies permission management, especially with employee job changes.


Example: Ralph changes roles from Finance to Facilities to HR (Figure 2).
His access is adjusted based on his new role (Finance -> Facilities -> HR).

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/a0c0e335-2ca8-41e9-b31f-49a55de31074)

# BENEFITS OF ROLE-BASED ACCESS

* Easier to maintain permissions and ensure consistency.
* Users only have access to data required for their current role (data security).
* Simplifies permission audits for compliance.

# RISKS OF USER-BASED ACCESS

* Assigning permissions directly to users is risky and complex.
* Increases chance of errors, like forgetting to remove old permissions (Figure 3).
* Can lead to users having too much access (security risk).


![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/664f41ea-3cbe-465e-8766-a658da85908d)

# Group Permissions

When developing a role-based access strategy, it is common to implement user group-based permissions.

EXAMPLE OF SAMPLE ORGANIZATION CHART

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/fcf79a65-61f6-4560-ad05-18a4aa9d4fae)

# Data Use Agreements

A Data Use Agreement (DUA) is a contract between organizations that outlines the rules for sharing private data.  It's important to have a DUA in place before you give any private data to another organization. When creating a DUA, you need to consider how sensitive the data is. The more sensitive the data, the stricter the rules in the DUA should be about how it can be shared.

# example of group based roles
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/87f2c7a2-6ad4-4320-b610-363270393377)


# DUA: Rules for Sharing Private Data

* A DUA is a contract that sets the rules for securely transferring, using, and disclosing private data between organizations.
* It specifies details like:
  * Who receives the data
  * How the data can be used (restrictions may apply)
  * How the data is transferred
  * How the recipient protects the data
  * No further distribution of the data without permission
* DUA approval processes vary by organization.
* Legal and regulatory requirements may influence the process.
In the US:
IRB approval needed for research on human subjects (FDA)
HIPAA compliance required for sharing protected health information


# Security Requirements


* Encryption scrambles data using a key, making it unreadable without the key. This protects data at rest (stored) and in transit (moving).
* Encryption Key: A secret code used for encryption and decryption. Losing the key makes the encrypted data inaccessible.
  
# Securing Data at Rest

* Databases are easier to secure due to centralized storage and access controls.

  * Transparent Data Encryption (TDE) encrypts database files for additional 
   security (e.g., Oracle and Microsoft offer TDE).
* Flat Files (on portable devices) pose a bigger challenge due to the risk of physical loss.

  * Device Encryption protects flat files if the device is lost or stolen (as long 
    as the encryption key is safe
    Securing Data in Transit

* HTTPS (Hypertext Transfer Protocol Secure): Encrypts the connection between two locations transferring data.
  * Combines HTTP (data transfer protocol) with TLS (Transport Layer Security) for encryption.



# EXAMPLE OF ENCRYPTED NETWORK CONNECTION 
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/f004d9c0-716a-4195-9172-bfa8e4cdafc8)

When a person navigates the Internet using a web browser, a padlock shows up in the address bar to indicate an encrypted HTTPS connection.

# EXAMPLE OF PADLOCK
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/5b2a83fe-e902-426d-84df-56bc681525a5)


ETL processes copy data between transactional and analytical systems. When copying files between the transactional and analytical servers, use the Secure Copy Protocol (SCP) or the Secure File Transfer Protocol (SFTP). As their names imply, both SCP and SFTP establish an encrypted tunnel to copy data

# EXAMPLE OF ETL PROCESS 

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/c25ab663-5018-433f-8dc1-a5b66bc14a95)

# Data Masking:

* Data masking replaces sensitive data elements (like Social Security numbers) with fake but realistic data in non-production environments (testing, training).
* This protects real people's privacy and reduces risk for the organization.
* Masking doesn't affect the usefulness of data for testing or training purposes (e.g., using a fake SSN for testing doesn't impact the test)


  # Data masking ETL process
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/2bccaa45-2fb4-4926-90b6-8b5a7e4541ab)

# DATA GOVERNANCE ACCELERATOR 

# CHAPTER 1: DEFINING DATA GOVERNANCE

Chapter focuses on:

* Unpacking the definition of data governance
* Discovering the elements of a data governance program
* Understanding the role of data culture
* Determining data governance readiness.

# UNDERSTANDING DATA GOVERNANCE
What is data governance: proactively managing your data inorder to support your organization to achieve its strategy and objectives. This is done by improving the quality of your data(Data governance: is simply a framework that you can use to proactively manage your data.

Inorder to be sucessful your framework needs the following 3 things:
* Policy: to mandate how your organization is going to manage data
* roles and responsibility :concernig data
* processes: detailing what needs to be done to manage data.

# WHAT IS MENT BY DATA GOVERNANCE?

Governance is a manner in which entity chooses to oversee the control and direction of an area of interest. it typically takes the form of how decisions are made, regulated, and enforced. when entitiesgrow and increase in complexity, formal governance becomes important. Left ungoverned, the possibility of developing into chaos is very probable

Governance is the system that formalizes control, processes, and accountabilities so that specific results such as meeting goals or sustaining standards can be attained.

# laws

The formality and structure that governance takes depend on context and intent. For example, given their goals as organizations, governance in a public agency such as a city will differ greatly from that of a private enterprise. Each of these entities has different purposes and responsibilities.

# Importance

* Well-managed data can be transformational, and it can support the desirable qualities of a data-driven culture. This is when decisions at all levels of the organization are made using data in an informed and structured manner such that they deliver better outcomes internally and to customers
  
*Successful data governance also means that data risks can be minimized, and data compliance and regulatory requirements can be met with ease. This can bring important comfort to business leaders who, in some jurisdictions, can now be personally liable for issues arising from poor data management.


# Data Governance Versus Data Management

* Data governance: sets the rules for how data is handled within an organization. This includes things like who is responsible for different data sets, what policies are in place to ensure data quality, and how data is measured and tracked throughout its lifecycle.
  
# Data management: is the practical side of things. It's about using technology and tools to implement the data governance rules. This includes things like building databases and data warehouses, securing data with encryption, and analyzing data to make informed decisions.

# Data Governance versus Information Governance

* Data governance: deals with the data itself, regardless of its specific meaning. It focuses on policies and procedures to ensure things like data security, for instance, for patient or staff data. Here, the emphasis is on protecting the data, not its specific use in the business.
  
* Information governance: on the other hand, is all about the meaning and context of data. It looks at how data relates to each other and how it can be used to generate value for the organization, customers, and stakeholders.


# The Value of Data Governance

* Data is seen as critical for success by many businesses. (statistic cited)
  
* Organizations that implement processes to manage data effectively show a commitment to data governance. This involves controlling and being accountable for how data is used.

# SOME OF THE MAIN ADVANTAGES ACHIEVED BY GOOD DATA GOVERNANCE:
* Improved data quality
* Expanded data value
* Increased data compliance
* Improved data-driven decision-making
* Enhanced business performance
* Greater sharing and use of data across the enterprise and externally
* Increased data availability and accessibility
* Improved data search
* Reduced risks from data-related issues
* Reduced data management costs
* Established rules for handling data

# CREATING A DATA GOVERNANCE PROGRAM
# The basic steps for creating a data governance program consist of the following:

*Defining the vision, goals, and benefits.
* Analyzing the current state of data governance and management.
* Developing a proposal based on the first two steps, including a draft plan.
* Achieving leadership approval.
* Designing and developing the program.
* Implementing the program.
* Monitoring and measuring performance.
* Maintaining the program.

Data governance is about managing data well and helping to deliver its optimum value to your organization. It includes ensuring your data is available, usable, and secure. It’s the actions that team members take, the policies and processes they must follow, and the use of technologies that support them throughout the data lifecycle in their organization. It’s safe to say that for a growing number of organizations, data governance is becoming a very big deal.

# THE MOST COMMON ELEMENTS OF DATA GOVERNANCE PROGRAM:
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/35a133bd-ac3e-4e33-b9d2-d2ade4195eb2)


# Developing a Data Governance Framework

A data governance framework is essentially a blueprint for how an organization manages its data. It's a set of rules, processes, and responsibilities that dictate how data is collected, stored, used, and protected. The goal is :

* High quality: Accurate, consistent, and reliable.
* Secure: Protected from unauthorized access or breaches.
* Compliant: Follows all relevant laws and regulations.
* Accessible: Available to those who need it for legitimate purposes.

# COMMON COMPONENTS OF A DATA GOVERNANCE FRAMEWORK


![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/5ae77893-f92d-4f6c-ae7c-c174c0cf6825)

* Roles and responsibilities: Who is accountable for different aspects of data governance? (e.g., data stewards, data quality specialists)
  
* Policies: Guidelines for how data should be handled (e.g., data security policies, data retention policies)
  
* Standards: Definitions and formats for data to ensure consistency (e.g., data dictionaries)
  
* Metrics: How will you measure the success of your data governance program? (e.g., data quality metrics)
  
* Processes: Specific procedures for handling data throughout its lifecycle (e.g., data cleansing procedures)

* Tools: There's a wide range of software to support data governance and management tasks.
These tools address various needs such as managing master data, creating data catalogs, data searching, data security, data integration, data analysis, and ensuring compliance with regulations.
Recently, data science tools have become easier to use and more automated, making data management less complex.
This improvement allows more people to participate in effectively managing data and extracting value from it.

* Communications and Collaboration; Data governance involves ongoing changes, so keeping everyone informed is crucial.
This communication can happen through various channels like meetings, emails, newsletters, and workshops.
Special attention needs to be paid to explaining how these changes impact different teams and their responsibilities within the data governance program.

# PREPARING FOR DATA GOVERNANCE

* Just setting up a team, plan, and buying tools isn't enough for successful data governance.
  
* Organizations need to assess if they're prepared for the cultural shift it entails.
  
* A key factor is having a data culture - how data is viewed and handled within the organization.
  
* A mature, data-driven culture is much more receptive to data governance than a reactive one where data handling is haphazard.
  
* Another crucial element for success is ensuring the organization's overall strategy aligns with the data governance program. Misalignment is a major reason for program failures.

WHAT IS DATA CULTURE?

* Impact on Success: A strong data culture is a critical factor for successful data governance implementation.  If employees don't understand the importance of data quality, security, and responsible use, data governance initiatives will likely face resistance and struggle to achieve their goals.

# Characteristics of a Good Data Culture:
A data-driven culture is characterized by:

* Data awareness: People recognize the value of data and its potential to improve decision-making.
  
* Data literacy: Employees have the skills and knowledge to understand, work with, and analyze data effectively.
  
* Data sharing: There's an openness to sharing data across departments to achieve organizational goals.
  
* Data accountability: People are held responsible for the quality and responsible use of data they handle.
  
* Data Governance Fosters a Data Culture:  While a strong data culture is essential for successful data governance, the process itself can also help cultivate those positive attitudes and behaviors. By setting clear policies, promoting data literacy programs, and demonstrating the value of data-driven decision making, data governance initiatives can influence how people view and interact with data throughout the organization.


# Assessing the Data Culture





# Maturing the Data Culture:

* Leadership champions data: Leaders need to actively communicate the importance of data and demonstrate its value through real-world examples of successful data-driven decisions.

* Empowering employees: Provide basic data skills training covering data manipulation, analysis, cleansing, querying, and visualization. Don't underestimate the power of common tools like spreadsheets for data management.

* Start small, celebrate progress: Focus on achievable steps to initiate the data culture journey.  Basic data management skills training can be a good starting point. Celebrate even small wins to keep momentum going.

* Embrace challenges:  Acknowledge that there will be resistance and frustration during this culture shift.  Focus on providing support mechanisms like open communication channels and positive discussions to address concerns and celebrate successes.

# Assessing Data Governance Readiness

Unfortunately, the success rate of data governance programs on the first try remains low. It’s important to maximize the conditions for success. You may not get a second chance.
# The following basic checklist of items will help you determine the data governance readiness of your organization:


# CHAPTER 2 
Overview
In this chapter, we will be:

* Defining data and its relationship to information
* Exploring the role of data in the 21st century
* Moving from data to insights
* Discovering the impact of big data

* Traditionally, organizations operate with limitations (budget, time, etc.). This scarcity is a fundamental principle in economics.
  
* However, the situation with data is quite different. Most organizations today have vast amounts of data collected through their activities, products, services, and interactions with customers and partners. This abundance of data, rather than limitations, presents a new challenge.
  
* Organizations are now faced with questions about harnessing the potential of this data, protecting it, and simply managing its sheer volume.
  
* We're living in the age of big data, and effectively managing this data can significantly improve an organization's performance and profitability.


# Defining Data

* Data refers to collections of digitally stored units, in other words, stuff that is kept on a computing device. These units represent something meaningful when processed for a human or a computer. Single units of data are traditionally referred to as datum and multiple units as data. However, the term data is often used in singular and plural contexts.

* Data is also defined based on its captured format. Specifically, at a high level, it falls into one of the following categories:

# Structured:
Data that has been formatted to a set structure; each data unit fits nicely into a table in a database. It’s ready for analysis. Examples include first name, last name, and phone number.

# Unstructured:
Data that are stored in a native format must be processed to be used. Further work is required to enable analysis. Examples include email content and social media posts.
# Semi-structured: 
Data that contains additional information to enable the native form

# Welcome to The Zettabyte Era

* In the past, the term "zettabyte" wasn't commonly used because data wasn't as prevalent.
  
* With the digital age and our increasingly connected world, the amount of data being created and stored has grown tremendously.
  
* To handle this massive amount of data, we've had to bring back the term "zettabyte" as a unit to measure this vastness.
  

 # The qualitative and quantitative nature of data types. 
 ![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/c76a3386-c841-4533-8f8c-4424e668e1e2)

 
* Zettabyte Era: We're in a time where data is measured in zettabytes - a vast unit equal to 1,000,000,000,000,000,000,000 bytes (written as 10^21).

* Explosive Data Growth: By 2020, we created 64 zettabytes of data, and this keeps growing rapidly. Projections estimate reaching over 100 zettabytes by 2023 and potentially doubling in just a few years.
  
* Perspective on Size: Imagine needing a billion terabyte drives to store just one zettabyte!
  
* Technical Breakdown: A zettabyte is made up of bytes, which are collections of 8 bits (0s and 1s) - the fundamental building blocks for storing data on computers.
  
* Future of Data Measurement: As data keeps growing, we might need even larger terms like yottabyte and brontobyte to measure it.

# Quantification of Data Storage

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/60cfd1e1-1bc2-4b24-86a9-67263944dc80)




# Examples of Data Volumes
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/bea1e209-c49f-46c2-a6e3-c7cb03f8f601)

Managing a small amount of data can have challenges, but managing data at scale is materially more challenging. If you’re going to glean value from data, it has to be understood and managed in specific ways.

# From Data to Insight

* Simply collecting and storing data isn't valuable. It needs to be done with a specific purpose or intended future use in mind.
  
* There might be some rare exceptions where collecting data without an immediate use case makes sense, but this shouldn't be the norm.
  
* In most cases, organizations collect data because it's essential for a particular goal or function.

# The Differences Between Data and Information

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/c4323b57-c8fc-4a94-97aa-6880101a9d19)


* Data is the raw, unprocessed information we collect.
* Information is data put into context, making it more meaningful.
* Knowledge is what you can do with information. It's actionable and allows you to understand how to use information for a specific purpose. This is where the saying "knowledge is power" comes into play.
* Wisdom builds upon knowledge. It involves applying reasoning, values, and broader life experiences to make sound judgments about the validity and application of knowledge in different situations. Not all knowledge is wisdom, but all wisdom includes knowledge.
* Insight is the deepest level of understanding. It combines knowledge and wisdom to see something in a new light and gain a deeper understanding. It allows you to think or see things differently.


# To summarize, consider the following:

* Harry Styles is data.
  
* The fact that Harry Styles is a singer and was in the group, One Direction, is information.
  
* The fact that Harry Styles has aspirations to become a solo artist and is looking for a record deal is knowledge.
  
* The fact that One Direction was a very successful band with talented and popular individuals and knowing that Harry Styles is a creative artist who now wants a solo record deal is wisdom.
  
* Ensuring that Columbia Records make the decision to sign Harry Styles before anyone else does is insight.

# Below illustrates the journey from data to insight.

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/da1020a5-ab58-441b-b390-4fcd95f3f937)


Another depiction of the data-information-knowledge-wisdom (DIKW) hierarchy as a pyramid to manage knowledge is illustrated below:

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/58e9e9ac-f4f8-494d-9949-a138ec50f36a)


* Different organizations can have varying results even when analyzing the same data set.
* There's no guaranteed path to the "best" outcome, regardless of the tools, processes, or skills used.
* However, good data governance practices can significantly improve the results you get from your data.

# The Role of Data in the 21st Century

* Data's Consistent Value: Data has always played a crucial role in helping us understand the world, make better decisions, and solve problems.
  
* The Data Explosion: Since the mid-20th century, the rise of computers significantly increased the volume, quality, and accessibility of data.
  
* The Information Age: The internet's arrival in the mid-90s made information readily available, fulfilling the vision of "information at your fingertips."
  
* Democratization of Information: Bill Gates' vision of accessible information for everyone further emphasized the growing importance of data in the late 1980s.

* Data Deluge: We're producing more data than we can manage. This vast data, with its depth, breadth, and quality, is transforming various aspects of our lives.
* Impact on Industries and Cities: This data revolutionizes the tools and capabilities of our industries and cities.
* Societal Shifts: It's fundamentally changing how we learn, socialize, and entertain ourselves.
* Heightened Risks: Cybersecurity threats are no longer minor inconveniences. A cyberattack can now cause significant financial losses within a short time frame.


# Data-Driven Decision-Making

* Data for Personal Choices: We use data in everyday decisions, like reading online reviews to choose a restaurant. This data is valuable to both consumers (informing decisions) and businesses (gaining customer feedback).
  
* Data for Complex Decisions: Businesses use vast amounts of data to make complex choices, like entering new markets. Analyzing this data helps make well-informed decisions and avoid costly mistakes.
  
* Data Makes a Difference: Access to good data and the ability to analyze it are crucial for making sound decisions. Without this, businesses risk making poor choices.

IMPORTANT
* Good Data Makes Good Decisions: Having a lot of data is helpful, but it needs to be accurate and reliable (good quality) to make sound decisions.
  
* Quality Over Quantity: Bad data can lead to poor choices and challenges.
21st Century Data Abundance: We have a lot of data available now, but ensuring its quality requires specific actions.
  
* Data Governance for Quality: Data governance practices are essential for achieving good quality data.

# Data as The New Oil

* Data as the New Oil: This quote by Clive Humby emphasizes that data, like oil, is a valuable resource that fuels modern economies.
  
* Data Needs Processing: Just as oil needs refining to be useful, data requires processing and analysis to unlock its true potential.
  
* Extracting Value from Data: This processing involves organizing and analyzing data to identify patterns, make informed decisions, solve problems, and feed other systems.

# Without these additional steps of organizing and analyzing, oil and data are similar in that they are notably messy and unusable in their raw form.

the below passage compares data to oil and highlights its importance in the digital age:

* Data Fuels Digital Economies: Similar to how oil powered industrial economies, data is the driving force behind the digital economies of the 21st century.
  
* Tech Giants Lead the Way: Companies like Facebook and Google, with their vast data resources, are major players in this data-driven economy.
  
* Data Revolution Across Industries: Data and digitalization are transforming every sector, from banking and government to countless others.
  
* Data as a Profit Engine: Organizations are shifting data management from a cost to a profit center, using data to power their businesses and generate revenue streams.
  
* Power Imbalance and Risks: Just like oil, control of large amounts of valuable data grants immense power. The historical dependence on oil highlights potential risks associated with a few big players managing personal data.

# Data Ownership

* Effective management requires assigning clear responsibility. This is done through job descriptions and project roles.
  
* Similarly, data accountability is crucial. Every data set within an organization needs to have someone responsible for it.

* This concept shouldn't be surprising, as it aligns with established management practices.

# The passage defines data ownership and the varying levels of control it entails:

* Data Ownership refers to the rights and control exercised over a particular data set by ana individual, team, or organization.
* Spectrum of Control: This control can range from basic oversight to strict, legally binding rules.
* Example: Intellectual Property: Data related to intellectual property (copyrights, trade secrets) will typically have strong ownership protections, including restrictions on access, usage, and purpose.


# DATA ARCHITECTURE

* Technology is Essential: Nearly every organization relies on technology to operate and deliver products or services. They can be considered technology businesses in this sense.
  
* Enterprise Architecture (EA): This framework helps organizations design, plan, and implement the right technology solutions (systems, policies, projects) aligned with their overall business strategy. It uses established standards and principles.
  
* Data Architecture as a Subset of EA: Just like EA focuses on the bigger picture of technology aligning with strategy, data architecture focuses specifically on how data is designed and managed to support both EA and the overall business goals.
  
* Data Architecture Blueprint: In simpler terms, data architecture is the agreed-upon plan for how data structures and management practices will support the organization's functions and technologies.

IMPORTANT
* Strong Architectures, Smooth Operations: When both EA and data architecture are implemented effectively, organizations can function more efficiently and adapt to changing circumstances (internal or external).
  
* The Downside of Weak Architectures: Poor or missing architectures can hinder digital transformation efforts, introduce complexity, and increase the risk of failure.
  
* Working Together: By design, these architectures work together to ensure data supports the organization's technological needs and overall business strategy.

# fIVE KEY OBJECTIVES OF DATA ARCHITECTURE

1. Data Accessibility: Ensuring the right people have access to the data they need to do their jobs, while also controlling access for security purposes.

2. Data Usability: Simplifying how people can find, understand, and use data within the organization.
   
3. Data Protection: Implementing safeguards to protect data in accordance with organizational policies and legal requirements.
   
4. Data Standardization: Establishing consistent data formats and definitions to ensure clear and consistent data use across the organization.
   
5.Data Efficiency: Optimizing data flows to eliminate redundancy, bottlenecks, and wasted resources.

# The passage highlights the connection between data governance and data architecture:

* Data Architecture Reflects Governance: A well-defined and functioning data architecture indicates an organization prioritizes data. It's managed as a valuable asset with controls to ensure alignment with business needs.
  
* Shared Responsibility: Similar to enterprise architecture, data architecture isn't solely a technical concern. It's a responsibility shared across the organization.
  
* Data Flow and Silos: In medium to large organizations, data needs to seamlessly flow across departments (e.g., sales and product development) and serve diverse users in various formats. Data architecture helps achieve this.

# THE LIFE CYCLE OF DATA
All data goes through phases during its lifecycle
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/f05e9dab-01bf-4121-a02a-fc97466299d3)

FIVE STAGES OF THE DATA LIFECYCLE:

1. Creation: This is the origin of data. It can be generated manually or automatically, internally or externally, through various activities and system interactions.
   
2. Storage: Once created and intended for future use, data needs to be stored. This often involves databases residing on local drives, servers, or cloud storage solutions.
   
3. Usage: Data is typically collected and stored for a reason - to be used later, possibly for analysis. Before use, data may require processing to cleanse errors, convert formats, or manage access permissions.
   
4. Archiving: Here, data identified as inactive gets moved to a long-term storage system outside the active environment. This archived data can still be retrieved and used if needed in the future.
   
5. Destruction: While some might prefer to hold onto everything indefinitely, there comes a point when data destruction is necessary. This could be due to regulations, policies, or simply no longer needing the data. Destruction ensures data becomes inaccessible and unreadable, sometimes involving physical destruction of storage devices.

# IMPORTANCE! 

* Data Lifecycle Stages: Data exists in various states throughout its lifecycle (creation, storage, usage, archival, destruction).
  
* Stage-Specific Treatment: Data requirements and handling differ depending on the lifecycle stage. For instance, security measures for actively used data will be stricter compared to archived data.
  
* Data Governance Impact: Understanding the data lifecycle is crucial for data governance as it helps determine appropriate handling practices at each stage.
  

# UNDERSTANDING THE IMPACT OF BIG DATA

















