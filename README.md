## 🎯 Project Objective:-
The CFSAN Adverse Event Reporting System (CAERS) is a critical surveillance database maintained by the FDA, capturing adverse event and product complaint reports related to foods, dietary supplements, and cosmetics. This project focuses on analyzing CAERS data spanning 2004 to Q2 2017 to uncover meaningful insights into product safety and public health risks.

The primary objective of this analysis is to understand patterns and trends in reported adverse events, including how they vary across product categories, demographics, symptoms, and outcomes. By leveraging standardized MedDRA-coded terminology, the project aims to support regulatory monitoring, risk identification, and evidence-based decision-making that can ultimately contribute to improved consumer safety and public health outcomes.

## 📊 Dataset Overview

The dataset consists of FDA-submitted adverse event reports associated with food products, dietary supplements, and cosmetics. Each record represents a single report and includes detailed information about the product, patient, and event.

### Key Fields in the Dataset:

##### --> RA_Report # – Unique identifier for each adverse event report

##### --> RA_CAERS Created Date – Date the report was recorded in CAERS

##### --> AEC_Event Start Date – Date the adverse event began

##### --> PRI_Product Role – Indicates whether the product was a suspect or concomitant

##### --> PRI_Reported Brand/Product Name – Reported product name

##### --> PRI_FDA Industry Code & Name – FDA industry classification (e.g., Bakery Products, Ice Cream, Cosmetics)

##### --> CI_Age at Adverse Event – Age of the affected individual

##### --> CI_Age Unit – Age measurement unit (years, months, etc.)

##### --> CI_Gender – Gender of the individual

##### --> AEC_One Row Outcomes – Event outcomes such as hospitalization, ER visit, or non-serious illness

##### --> SYM_One Row Coded Symptoms – MedDRA-coded symptoms associated with the event

## 📈 Data Preparation & Modeling Approach

Raw data was cleaned and standardized using Power BI Power Query

Derived columns such as Age in Years, Event Start Date, and Report Created Date were created for consistent analysis

A star schema data model was implemented to ensure efficient relationships and optimized performance

DAX measures were developed to calculate event counts, demographic distributions, and outcome frequencies

## 🔍 Key Insights from the Dashboard

#### 1:- High Reporting Volume: The dataset contains ~65K adverse event reports, indicating substantial consumer safety concerns across food, supplement, and cosmetic products.

#### 2:- Demographic Risk Pattern:

Females account for ~63% (41K) of reports, significantly higher than males (~30%), suggesting gender-specific exposure or reporting behavior.

The median patient age is 52 years, with the 36–75 age groups contributing the highest number of adverse events.

#### 3:- Industry-Level Concentration:

Vitamins, Minerals, Proteins & Supplements dominate reporting (~28K reports) and show a notable number of serious outcomes, making this the highest-risk industry segment.

Cosmetics and certain food categories contribute fewer reports but are still associated with serious cases.

#### 4:- Outcome Severity:

Most reports are non-serious, but serious and fatal outcomes are consistently present across multiple industries, highlighting ongoing safety risks rather than isolated incidents.

#### 5:- Symptom Patterns:

A large variety of symptoms (5,549 unique symptoms) are reported, but a few dominate:
Diarrhea, vomiting, nausea, and abdominal pain are the most common—indicating strong gastrointestinal impact across products.

#### 6:- Trend Over Time:

Report volumes increase steadily over the years, with visible spikes after 2013, reflecting either increased product usage, better reporting awareness, or regulatory changes.

#### 7:- Growth & Risk Indicators:

Although the overall growth rate is slightly negative (-0.43%), the serious outcome rate (~0.9%) confirms that high-impact cases still persist and require monitoring.


