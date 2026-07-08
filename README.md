# CODEALPHA-EDA-ANALYSIS (OLYMPIC ANALYSIS)

# Section A :Project Overview 
The aim of the project is to basically gain a deeper understanding of the underlying patterns,facts and outliers regarding this Olympic Players data set .It explores participlation trends for countries,athlete details and facts regarding medals for both the Summer and Winter Games.The project showcases data cleaning,data visuals and most importantly Exploratory Data Analysis from over 271,000 athlete records 

### PROJECT QUESTIONS

##### 1.To what extent does the significant gender disparity (67.6% Male) seen in overall participation have effect across the top ten sports?

##### 2.What is the connection between an athletes physical characteristics  (Height and Weight, post-cleaning) and the possiblity of being categorized in a low participation sports over a high participation sports ?

##### 3.How does the exit of records with missing physical features (Age, Height, Weight) affect the representation of the top five participating countries in the world ?

# SKILLS SHOWCASED IN THIS PROJECT

I.Data Importation

II.Data Cleaning

III.Summary Statistics

IV.Creation of Data Visuals /Graphs and Charts 


# Section B: Dataset Description

The dataset athlete_events.csv contains 271,116 athlete records with 15 features covering:
ATHLETE INFORMATION

•	ID: Unique identifier for each athlete

•	Name: Athlete's full name

•	Sex: Gender (M/F)

•	Age: Athlete's age during the games

•	Height: Athlete's height in centimeters

•	Weight: Athlete's weight in kilograms

•	Team: Country/team represented
GAMES INFORMATION
•	NOC: National Olympic Committee 3-letter code

•	Games: Year and season of the games

•	Year: Year the games were held

•	Season: Summer or Winter

•	City: Host city of the games
SPORTS INFORMATION

•	Sport: Sport category

•	Event: Specific event within the sport

•	Medal: Medal won (Gold/Silver/Bronze/NaN)

# Section C: Methodology

DATA CLEANING & PREPROCESSING

1. Missing Values Treatment
2. 
•	Initial missing value count:

o	Age: 9,474 missing values

o	Height: 60,171 missing values

o	Weight: 62,875 missing values

o	Medal: 231,333 missing values (expected, as not all athletes win medals)

•	Data Imputation Strategy: Rows with missing values in Age, Height, or Weight were dropped to maintain data integrity for numerical analysis.

4. Duplicate Removal
5. 
•	Identified 60,800 duplicate rows in numerical columns

•	Retained 206,165 clean records for analysis

7. Column Optimization
   
•	Removed irrelevant columns: ID, City (not needed for core analysis)

•	Final dataset: 206,165 rows × 13 columns

# Section D: Summary Statistics
Key Metrics After Cleaning:

Metric	Value

Total Athletes	206,165

Average Age	25.56 years

Average Height	175.34 cm

Average Weight	70.70 kg

Male Athletes	139,454 (67.6%)

Female Athletes	66,711 (32.4%)

Year Range	1896 - 2016
Top Participating Countries:

1.	United States: 13,714 athletes
2.	France: 7,807 athleteS
3.	Canada: 7,668 athletes
4.	Great Britain: 7,499 athletes
5. Italy: 7,433 athletes
Top Sports:

1.	Athletics: 32,374 participants
2.	Swimming: 18,776 participants
3.	Gymnastics: 18,271 participants
4.	Rowing: 7,790 participants
5.	Cycling: 7,775 participants
   
# Section E: Key Visualizations
1. Top 10 Participating Countries
•	Visualization Type: Horizontal Bar Chart
•	Key Insight: United States leads with over 13,700 athletes, significantly outpacing other nations. The top 5 countries all have 7,400+ participants.
2. Age Distribution Histogram
•	Visualization Type: Histogram with KDE overlay
•	Key Insight: Athlete ages are concentrated between 16-40 years, with a normal-like distribution. This validates the typical athletic career span and peak performance ages.
3. Gender Distribution Pie Chart
•	Visualization Type: Pie Chart
•	Key Insight: Male athletes represent approximately 67.6% of participants compared to 32.4% female athletes, highlighting historical gender participation gaps in Olympic history.
4. Top 10 Sports by Participation
•	Visualization Type: Line Chart
•	Key Insight: Athletics dominates with over 32,000 participants, more than double the second most popular sport (Swimming with ~18,800 participants).
5. Statistical Summary Table
•	Comprehensive Overview: The describe() method provides detailed statistical information for numerical features including count, mean, standard deviation, min, max, and quartile values for each attribute.

# Section F: Technologies Used

Library	Purpose

Pandas	Data manipulation, cleaning, and analysis

Matplotlib	Basic plotting and visualization

Seaborn	Statistical data visualization with enhanced aesthetics

NumPy	Numerical operations and array handling

Jupyter Notebook	Interactive development and analysis environment

# CODE_ALPHA_DATA_VISUALISATION/
text
├── athlete_events.csv              # Main Olympic dataset

├── I.CODE ALPHA EDA ANALYSIS.ipynb # Complete EDA notebook

├── README.md                       # Project documentation

└── noc_regions.csv                 # NOC region mapping file

