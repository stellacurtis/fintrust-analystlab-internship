# Week 1 — Data Analytics Track
## FinTrust Digital Bank Experience Lab Project (AnalystLab Africa Internship)

---

## Part 1: General Week 1 Requirements

### A. Business Understanding

**1. What problem is FinTrust trying to solve?**

FinTrust is generating increasing volumes of customer and transaction data as more customers adopt its digital banking services. However, the bank currently lacks an effective approach for analysing this data and turning it into actionable insights. This makes it difficult to identify unusual transaction patterns, understand customer behaviour, assess potential risks, and monitor operational performance. As a result, decision-makers may not have timely, data-driven information to support effective risk management, improve customer experience, and strengthen overall banking operations.

**2. Why is the problem important?**

The problem is important because without effective use of its customer and transaction data, FinTrust may struggle to make timely and informed business decisions. As transaction volumes increase, the inability to identify important patterns and potential risk indicators could expose the organisation to financial losses and make it more difficult to detect unusual transactions that may require further review.

The gap could also affect customer experience and trust. If FinTrust does not adequately understand customer behaviour or transaction issues, it may be harder to identify customer needs, improve services, and provide effective support. This could reduce customer satisfaction and make it more difficult for FinTrust to compete with digital banking organisations that use data to improve their services.

From an operational perspective, relying on limited or delayed insights could result in inefficient decision-making and make it harder for management to monitor performance and respond to emerging issues. In addition, as a financial institution, FinTrust would need reliable information to support appropriate risk monitoring and compliance-related processes. While this project does not make regulatory or legal claims, stronger data analysis would provide a better foundation for monitoring potential risk indicators and supporting responsible decision-making.

**3. How can the Data Analytics track contribute to solving it?**

The Data Analytics track can help address FinTrust's information and decision-making gaps by analysing customer and transaction data to provide clear visibility into customer behaviour, transaction activity, and transaction patterns. By identifying meaningful trends, differences across customer groups, and potentially unusual or higher-risk transaction patterns, the analysis can help management better understand what is happening across the business.

The track will also develop relevant KPIs to support the monitoring of customer and transaction performance and present key findings through a dashboard. This will give decision-makers a clearer and more accessible view of the data, helping them make informed decisions related to customer needs, operational performance, and risk-related areas.

Overall, the Data Analytics track will transform FinTrust's raw data into structured insights that can support better visibility, customer understanding, and data-driven decision-making.

**4. What type of output could the Data Analytics track provide?**

- A Business Understanding document
- A Data Understanding and Profiling Report
- A set of 5–8 analytical questions
- A KPI Definition Table
- A Dashboard Wireframe showing proposed KPIs, visuals, filters, and key insights
- An Initial Analysis Plan for Weeks 2–4
- A final analytical dashboard and business insights based on the findings

---

### B. Review of Relevant Resources

**Resource 1: FinTrust Customer Data**

*What it contains:* The FinTrust Customer Data contains information about 1,500 customers, including demographic characteristics such as age, gender, and city; customer and account information such as customer segment, account type, tenure, and account status; and behavioural information such as digital engagement score and preferred channel. It also contains customer identification information, including Customer_ID and Customer_Name.

*How I will use it:* I will use this dataset to understand customer characteristics and examine how customer demographics, account characteristics, and digital engagement relate to their banking and transaction behaviour. Variables such as Customer_Segment, Account_Type, Tenure_Months, Digital_Engagement_Score, and Preferred_Channel can help answer questions about customer engagement, segmentation, and digital banking behaviour. The Customer_ID will also allow the customer information to be linked to the transaction dataset for further analysis.

*Limitations:* One limitation is that the dataset does not contain some potentially useful information about the customer experience, such as customer complaints, satisfaction, or reasons for using or leaving a service. Monthly income is provided as an income band rather than an exact income value, which limits more detailed income analysis. The presence of Customer_Name also raises a privacy consideration, so this field may not be necessary for most analytical tasks and should be handled appropriately.

**Resource 2: FinTrust Transaction Data**

*What it contains:* The FinTrust Transaction Data contains 12,000 transaction records and provides information about customers' banking transactions. It includes transaction details such as the date and time, transaction type, amount, channel, device type, and location. It also contains information about whether a transaction was international, its status, and whether it was flagged for risk review.

*How I will use it:* I will use this dataset to analyse transaction activity, transaction values, channel usage, and transaction patterns. Variables such as Amount_NGN, Transaction_Type, Channel, and Transaction_DateTime can help assess transaction volumes, values, and trends over time. Device_Type, Location, and International_Transaction can be used to examine behavioural and potentially unusual transaction patterns. Transaction_Status and Risk_Review_Flag can also help investigate transaction failures and potential risk patterns. The Customer_ID can be linked with the Customer Data to analyse transaction behaviour by customer characteristics and segments.

*Limitations:* The dataset does not provide information about the reason why a transaction was flagged for risk review, so the underlying cause of a risk flag cannot be determined directly. It also does not appear to contain a transaction fee field, meaning transaction costs or fee-related revenue cannot be analysed from these records. There is no merchant or merchant-category field, which limits analysis of where customers spend their money or which types of merchants are associated with transactions. In addition, the available fields may show that a transaction was successful, failed, or flagged, but may not explain the specific reason for the outcome.

**Resource 3: FinTrust Data Dictionary**

*What it contains:* The FinTrust Data Dictionary is a reference document that provides descriptions and supporting information for the Customer and Transaction datasets. It contains three tabs: Customer_Dictionary, Transaction_Dictionary, and Project_Notes. The Customer and Transaction Dictionary tabs provide information such as field names, dataset names, data types, examples, definitions, business uses, and modelling uses.

*How I will use it:* I will use the Data Dictionary throughout the project to understand what each field means, confirm the expected data type and interpretation of variables, and understand how the fields may be relevant to business and modelling objectives. I will also refer to it when cleaning and preparing the data to ensure that variables are handled according to their intended definitions. The Project Notes will be used to identify any project-specific instructions, assumptions, or known data limitations that should be considered during the analysis.

*Limitations:* The datasets are fictional and synthetic, so findings from the analysis should not be interpreted as representing actual FinTrust customers or real-world banking behaviour. In addition, Risk_Review_Flag is a synthetic educational target and does not represent a confirmed fraud determination. Therefore, any risk-related findings should be described as patterns associated with the synthetic risk-review label rather than evidence of actual fraud or financial risk. The Data Dictionary also notes that some Device_Type and Location values are intentionally missing for data-quality practice. These missing values should therefore be recognised and handled during data preparation, but should not automatically be treated as accidental data-entry errors.

---

### C. Track Objectives

1. To profile and explore FinTrust's customer and transaction data in order to understand data quality, structure, and relationships between datasets.
2. To identify key analytical questions and explore patterns in customer and transaction data in order to generate actionable insights for FinTrust.
3. To develop relevant key performance indicators (KPIs) in order to measure customer activity, transaction performance, and overall digital banking performance.
4. To design a dashboard wireframe that presents key metrics and insights in order to support clear and effective decision-making by FinTrust stakeholders.
5. To explore patterns associated with FinTrust's risk-review labels in order to identify trends that may support further risk monitoring and investigation.

---

### D. Success Criteria

- **Data profiling:** Success means the datasets are clearly understood, key data-quality issues are identified, and the relationships between the datasets are well documented.
- **Analytical insights:** Success means the analysis answers the key business questions and produces clear, evidence-based insights that can support FinTrust's decisions.
- **KPIs:** Success means each KPI is measurable using the available data, clearly defined, and directly linked to a relevant business question or objective.
- **Dashboard:** Success means the proposed dashboard presents the most important KPIs and insights clearly, allowing stakeholders to quickly understand performance and identify areas that need attention.
- **Risk patterns:** Success means potential patterns in risk-related data are identified and presented clearly enough to support further monitoring or investigation.

---

### E. Initial Plan for Weeks 2–4

**Week 2 — Data Preparation & Initial Analysis**
I will focus on deeper data cleaning, validation, and preparation of the customer and transaction datasets for analysis. I will also begin developing the initial KPIs and exploring key patterns, while collaborating with the other tracks to understand how the Data Analytics outputs can support the wider FinTrust solution.

**Week 3 — Analysis & Dashboard Development**
I will conduct deeper analysis to answer the identified business questions and refine the KPIs based on the findings. I will then develop and refine the dashboard structure and visualisations to ensure that the most important metrics and insights are presented clearly and effectively.

**Week 4 — Refinement, Integration & Final Delivery**
I will validate and polish the analysis, KPIs, and dashboard based on feedback from stakeholders and other project tracks. I will finalise the key insights and documentation, ensure the Data Analytics outputs align with the overall FinTrust solution, and prepare the work for final presentation.

---

## Part 2: Data Analytics Track — Business & Data Intelligence Assessment

### Part A — Business Understanding

**1. What business questions should FinTrust's management be able to answer?**

- How many active customers does FinTrust have, and how does customer activity change over time?
- What are the transaction volumes and values across different transaction types, channels, and customer segments?
- Which customer segments and transaction channels contribute most to FinTrust's overall transaction activity?
- What trends or unusual changes can be observed in customer activity and transaction performance?
- Which areas of the business are performing well, and where are there potential areas for improvement?
- What patterns can be observed in transactions associated with different risk-review labels?
- How do customer characteristics and behaviour relate to transaction activity and performance?

**2. What decisions could data analysis support?**

- **Resource allocation:** Decide which customer segments, transaction channels, or areas of the digital banking service require more resources or investment based on performance.
- **Customer engagement:** Identify customer groups with low or declining activity and inform targeted engagement or retention strategies.
- **Channel and operational improvements:** Determine which transaction channels are performing well or experiencing issues and guide decisions on where operational improvements are needed.
- **Risk monitoring:** Prioritize transaction patterns or customer segments that show higher levels of risk-related activity for further review and monitoring.
- **Performance management:** Use KPI trends and dashboard insights to determine whether business performance is improving and where corrective action may be required.

**3. What stakeholders could benefit from the analytical outputs?**

- **Senior Management:** Use dashboards, KPIs, and insights to monitor overall business performance and support strategic decision-making.
- **Operations Team:** Use transaction and channel performance insights to identify operational issues and areas requiring improvement.
- **Risk and Compliance Team:** Use risk-related patterns and transaction trends to prioritize areas for further review and monitoring.
- **Product Team:** Use customer behaviour and transaction insights to understand how customers interact with FinTrust's services and identify areas for product improvement.
- **Data Science & Machine Learning Teams:** Use the cleaned and analysed data, identified patterns, and KPIs as a foundation for further modelling and predictive work.
- **Generative AI Team:** Use validated business insights and analytical findings to help inform relevant AI-powered features or support solutions.
- **Project Management Team:** Use the analytical outputs to track project objectives, communicate progress, and support coordination across the different tracks.

---

### Part B — Data Understanding and Profiling

The FinTrust dataset consists of two related datasets: Customer Data and Transaction Data. The Customer Data contains 1,500 records and 12 columns, while the Transaction Data contains 12,000 records and 11 columns. The two datasets are linked through Customer_ID, with each customer potentially having multiple transaction records. The 1,500 unique Customer_IDs found in the transaction dataset match the number of customers in the Customer Data, indicating that the datasets have good join integrity.

**Customer Data**

The Customer Data contains information about FinTrust customers, including Customer_ID, Gender, City, Customer_Segment, Account_Type, Monthly_Income_Band, Preferred_Channel, Account_Status, Age, Tenure_Months, and Digital_Engagement_Score.

The Customer_ID field is a unique identifier, with 1,500 unique values across the 1,500 records. The dataset contains no missing values, which indicates good completeness at the customer-data level.

The categorical variables include Gender, City, Customer_Segment, Account_Type, Monthly_Income_Band, Preferred_Channel, and Account_Status. Customer segments are divided into Premium, Everyday, SME, and Student, while account status consists of Active, Dormant, and Restricted. These variables can be used to compare customer behaviour and transaction activity across different customer groups.

The numerical variables include Age, Tenure_Months, and Digital_Engagement_Score. These variables can support analysis of customer characteristics, length of relationship with FinTrust, and level of digital engagement.

**Transaction Data**

The Transaction Data contains 12,000 transaction records and 11 columns. It includes information about transaction characteristics, channels, devices, locations, transaction outcomes, amounts, and risk-review status.

The categorical variables include Transaction_Type, Channel, Device_Type, Location, International_Transaction, Transaction_Status, and Risk_Review_Flag. Transaction Status is classified into Successful, Failed, Reversed, and Pending, while Risk_Review_Flag identifies transactions marked for risk review.

Amount_NGN is the main numerical variable and ranges from ₦100 to ₦693,454. The median transaction amount is ₦10,306, while the mean is considerably higher at ₦46,706. This large difference suggests that the transaction amounts are right-skewed, meaning that a relatively small number of high-value transactions may be substantially increasing the average. This should be considered when analysing transaction values, as the median may provide a more representative measure of a typical transaction.

The transaction dataset covers the period from 1 January 2026 to 31 March 2026, providing approximately one quarter of transaction activity for analysis.

**Missing Values and Data Quality**

The transaction dataset has 96 missing values in Device_Type and 96 missing values in Location. These missing values are intentional according to the data dictionary, so they should not automatically be treated as data errors. However, their presence should be considered when conducting analyses involving device or location.

The Customer Data has no missing values, indicating complete coverage across the customer-level variables. Overall, the datasets appear to have good structural quality, with clearly defined fields and a consistent Customer_ID relationship between the two datasets.

One area requiring further investigation is the distribution of Amount_NGN, given the substantial difference between its mean and median. Further analysis should determine whether the high transaction values represent legitimate customer activity or potential outliers.

Another useful data-quality check would be to compare Account_Status with transaction activity. For example, transactions associated with Dormant or Restricted accounts may require investigation to determine whether they are expected under FinTrust's business rules or indicate potential data or operational issues.

**Relationship Between the Datasets**

The Customer Data and Transaction Data have a one-to-many relationship through Customer_ID. Each customer appears once in the Customer Data, while the same Customer_ID can appear across multiple transaction records. This structure allows customer characteristics such as segment, income band, account status, and digital engagement to be combined with transaction behaviour.

This relationship provides the foundation for analysing questions such as how transaction activity differs across customer segments, whether digital engagement is associated with transaction behaviour, and how transaction patterns vary by account status or preferred channel.

---

### Part C — Analytical Questions

1. **Customer Behaviour:** How does transaction activity vary across customer segments, account types, and levels of digital engagement?
2. **Transaction Activity:** Which transaction types generate the highest number and total value of transactions during the January–March 2026 period?
3. **Transaction Value:** How does the average and median transaction amount vary across customer segments, transaction types, and channels?
4. **Transaction Channels:** Which transaction channels have the highest transaction volumes and values, and which channels have the highest proportion of failed or reversed transactions?
5. **Transaction Status:** What proportion of transactions are successful, failed, reversed, or pending, and how does transaction status vary across transaction types and channels?
6. **Risk Patterns:** Which transaction types, channels, customer segments, or transaction characteristics have the highest proportion of transactions flagged for risk review?
7. **Customer Activity Over Time:** How does transaction volume and value change over the three-month period, and are there noticeable peaks or declines in customer activity?
8. **Account Status:** Do Dormant or Restricted accounts show transaction activity, and if so, how does their transaction behaviour compare with Active accounts?

---

### Part D — KPI Definition Table

| KPI | Definition | Why It Matters | Required Data |
|---|---|---|---|
| Transaction Failure/Reversal Rate | Percentage of total transactions with Transaction_Status of Failed or Reversed. (Failed + Reversed transactions ÷ Total transactions) × 100 | Helps FinTrust monitor transaction reliability and identify channels or transaction types that may require operational investigation or improvement. | Transaction_Status, Transaction_ID |
| Average Successful Transaction Value | Average amount of transactions where Transaction_Status = Successful. Total value of successful transactions ÷ number of successful transactions. | Helps FinTrust understand the typical value of completed transactions and identify changes in customer spending or transaction behaviour. | Amount_NGN, Transaction_Status |
| Digital Channel Usage Rate | Percentage of total transactions conducted through each digital channel, such as Mobile App or USSD. | Shows which channels customers use most and can support decisions about channel investment and improvement. | Channel, Transaction_Status |
| Risk Review Rate | Percentage of total transactions flagged for risk review. (Risk-reviewed transactions ÷ Total transactions) × 100 | Helps FinTrust monitor the level of transactions requiring risk attention and identify segments or channels with higher risk-review activity. | Risk_Review_Flag, Transaction_Type, Channel, Customer_ID |
| Average Transactions per Customer Segment | Average number of transactions generated per customer within each customer segment. | Helps identify which customer segments are most active and can support customer engagement, retention, and resource-allocation decisions. | Customer_ID, Customer_Segment |

---

### Part E — Dashboard Wireframe

**Section 1: Overview**
- *KPI cards:* Transaction Failure/Reversal Rate, Average Successful Transaction Value, Digital Channel Usage Rate
- *Charts:* A line chart showing transaction volume and value over time, and a bar chart comparing transaction volume across channels

**Section 2: Customer Insights**
- *KPI cards:* Average Transactions per Customer Segment
- *Charts:* A bar chart comparing transaction activity across customer segments and a bar chart showing transaction value by segment

**Section 3: Risk & Transaction Performance**
- *KPI cards:* Risk Review Rate and Transaction Failure/Reversal Rate
- *Charts:* A bar chart showing failure/reversal rates by channel or transaction type, and a bar chart showing risk-review rates across customer segments or transaction types

**Filters:**
- Date range
- Customer segment
- Transaction type
- Transaction channel
- Transaction status

**Expected Insights:**
The dashboard should provide a quick view of FinTrust's overall transaction performance, customer activity, channel usage, and risk-review patterns. It should help stakeholders identify high-performing customer segments and channels, detect areas with higher transaction failure or reversal rates, and identify transaction patterns that may require further risk monitoring or operational attention.
