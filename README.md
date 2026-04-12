📊 EdTech User Acquisition & Funnel Conversion Analysis
📌 Project Overview
This project focuses on analysing user acquisition and funnel conversion behaviour for an EdTech platform using transactional and engagement data to uncover actionable business insights. The analysis aims to help stakeholders understand which channels and geographies drive the highest-quality users, where the conversion funnel loses potential students, and how to optimise marketing and product strategies to improve enrolment rates and revenue.
The project follows an end-to-end data analytics workflow, covering data merging and cleaning, exploratory analysis, SQL-based business queries, and interactive dashboarding.
🎯 Business Objectives

Identify and quantify drop-off at each stage of the user acquisition funnel
Evaluate channel-wise conversion performance across five acquisition sources
Analyse city-wise enrolment rates across eight major Indian metros and tier-2 markets
Assess revenue performance including total revenue and average order value
Understand device and demographic distribution to inform product and marketing decisions
Generate insights to support marketing budget allocation, geographic expansion, and product optimisation

🗂 Dataset Description
Total Records: 1,500 registered users; 225 paid enrolments
Total Columns: 16 across three relational tables
Data Includes:

User demographics (age, city, device type)
Acquisition channel (Instagram, YouTube, Referral, Google Ads, Website)
Engagement indicators (course viewed flag, demo attended flag)
Enrolment details (enrolment date, course ID, amount paid)

Data Quality Issues Addressed:

Null values in engagement flag columns filled with 0 for accurate funnel counts
Three tables joined on user_id using LEFT JOINs to preserve all registered users
Boolean enrolled flag derived from enrollment_date for downstream analysis

🛠 Tools & Technologies Used

Excel: Initial exploration and dataset familiarisation
Python: Data merging, preprocessing, funnel flag engineering, and EDA

Libraries: Pandas, Matplotlib


SQL (Google BigQuery): Business queries and funnel aggregations
Power BI: Interactive dashboards and KPI tracking
Git & GitHub: Version control and project documentation

🔄 Project Workflow
Data Understanding & Cleaning

Merged Users, Engagement, and Enrollments tables on user_id
Filled null engagement flags with 0
Derived binary enrolled flag from enrollment_date

Exploratory Data Analysis (Python)

End-to-end funnel count and visualisation (Signup → View → Demo → Enrol)
Stage-to-stage and overall conversion rate calculations
Device and age demographic profiling

SQL-Based Business Analysis

Overall funnel metrics (signups, views, demos, enrolments)
Channel-wise funnel breakdown and conversion rate comparison
City-wise funnel breakdown and enrolment rate ranking
Revenue summary: total revenue, average order value, enrolments

Dashboard Development (Power BI)

Funnel visualisation with user counts at each stage
Channel and city performance comparisons
Revenue and demographic KPI cards
Device distribution breakdown for product prioritisation

📈 Key Insights

The View-to-Demo stage is the largest funnel bottleneck, with only 44.8% of course viewers proceeding to attend a demo
Jaipur delivers the highest signup-to-enrolment conversion rate (21.4%), significantly above the 15% overall average
Instagram is the dominant acquisition channel by volume (517 signups, 79 enrolments), while Website-sourced users convert at the highest rate (15.9%)
Hyderabad has the lowest enrolment conversion rate (11.2%) despite near-average signup volumes, indicating a potential audience-product mismatch
Android accounts for 52.7% of the user base, making mobile-first optimisation a priority
The platform generated INR 11,07,775 in total revenue from 225 paid enrolments, with an average order value of INR 4,923

💡 Business Recommendations

Implement automated follow-up sequences (WhatsApp / email) for users who view a course but do not book a demo, targeting the View-to-Demo bottleneck
Increase marketing investment in Jaipur and other tier-2 markets where conversion rates exceed the platform average
Prioritise Android app performance to serve the majority device segment effectively
Conduct a cohort-level investigation into Hyderabad to diagnose the cause of its below-average conversion rate
Scale the Website / organic channel through SEO and content marketing to grow the highest-converting user source
Benchmark acquisition cost against revenue per signup by channel once CAC data is available to guide budget reallocation

📊 Dashboard Preview
The Power BI dashboard provides an interactive view of:

Funnel performance at each user journey stage
Channel-wise and city-wise conversion rate comparisons
Revenue KPIs and order value metrics
Device distribution and age demographic profile

(Dashboard file included in the repository)
