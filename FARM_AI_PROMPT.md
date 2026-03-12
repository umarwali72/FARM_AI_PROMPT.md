You are a professional livestock data scientist, herd geneticist, and agricultural software engineer.

Your task is to design a Python-based AI livestock management system for a goat breeding farm.

The system should function as a "Livestock AI Brain" that records farm data, analyzes herd performance, and predicts herd outcomes for the next 3 years.

The farm operates in Northern Nigeria under a semi-intensive system:
- goats graze freely during the day
- selected animals receive supplementary feed
- breeding is controlled to improve genetics
- herd size is expected to grow each year

The system must run offline on a basic laptop.

---------------------------------------

DATA STRUCTURE

The system must manage the following datasets:

1. Goat Register
Fields:
Goat_ID
Sex
Breed
Date_of_Birth
Color
Source
Purchase_Date
Purchase_Price
Status

2. Breeding Records
Fields:
Breeding_ID
Doe_ID
Buck_ID
Mating_Date
Expected_Kidding_Date
Actual_Kidding_Date
Number_of_Kids
Kids_Alive

3. Kidding Records
Fields:
Kid_ID
Dam_ID
Sire_ID
Birth_Date
Sex
Birth_Weight
Survival_Status

4. Weight Records
Fields:
Goat_ID
Date
Age
Weight

5. Health Records
Fields:
Goat_ID
Date
Condition
Treatment
Medication
Dose
Notes

6. Feed Records
Fields:
Date
Goat_ID_or_Group
Feed_Type
Quantity
Cost
Purpose

7. Sales Records
Fields:
Goat_ID
Date
Weight
Price
Buyer

8. Mortality Records
Fields:
Goat_ID
Date
Cause_of_Death

---------------------------------------

CORE FEATURES

The system must allow the farmer to:

Add new goats
Record breeding events
Track pregnancies
Record kidding events
Track kid survival
Track weight gain
Track feed supplementation
Record medical treatments
Record deaths and sales

---------------------------------------

ANALYTICS

The system must automatically calculate:

fertility rate
kid survival rate
average litter size
average daily weight gain
mortality rate
feed cost per goat
profit per goat

---------------------------------------

GENETIC MANAGEMENT

The system must:

track pedigree across generations
detect potential inbreeding
warn if related goats are bred
identify best breeding buck
identify best breeding doe

---------------------------------------

HERD INTELLIGENCE

The system should build performance scores for each goat:

Growth Score
Fertility Score
Survival Score
Health Score

Using these scores, identify:

Top breeding animals
Animals that should be sold
Animals that should not reproduce

---------------------------------------

PREDICTION SYSTEM

The Livestock AI Brain must simulate herd growth for the next 3 years using historical farm data.

Predictions should include:

Expected herd population
Expected number of kids
Expected mortality
Expected sales
Expected feed demand

---------------------------------------

REPORTS

The system must generate reports such as:

Herd population report
Breeding performance report
Growth performance report
Feed cost report
Mortality analysis
Genetic improvement report
3-year herd projection

---------------------------------------

TECHNICAL REQUIREMENTS

Use Python.

Use SQLite database for data storage.

Use pandas for data analysis.

Code should be modular and structured into components such as:

database manager
breeding manager
growth analyzer
genetics analyzer
feed analyzer
prediction engine
report generator

The system must work offline and be easy to expand.

Provide a simple command-line interface for interacting with the system.
