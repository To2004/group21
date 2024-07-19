# group21

# Instructions

1. **Download the dataset** from the provided link.

2. **Open RStudio** and ensure you have the necessary libraries installed.

3. **Place the downloaded file** in a directory of your choice.

4. **Update the file path** in the following R code to match the location where you saved the file:

    ```R
    data <- read.csv("/path/to/your/directory/tedsa_puf_2020.csv")
    ```

    Replace `"/path/to/your/directory/tedsa_puf_2020.csv"` with the actual path to the CSV file on your system.

5. **Run the code** in RStudio to load the dataset.

## Here is a high-level overview of the key elements and variables in the dataset:
## Detailed Column Descriptions


### AGE: Age at Admission
Description:
The variable represents the age of individuals at the time of their admission.
Categorization:
Age is categorized into different groups for analysis.
In the dataset:
1: 12-14 years old
2: 15-17 years old
3: 18-20 years old
4: 21-24 years old
5: 25-29 years old
6: 30-34 years old
7: 35-39 years old
8: 40-44 years old
9: 45-49 years old
10: 50-54 years old
11: 55-64 years old
12: 65 years and older


### GENDER: Categorical variable indicating the gender of the individual. Possible values are:
1: Male
2: Female
-9: Missing/unknown/not collected/invalid 


### RACE: Categorical variable indicating the race of the individual. Possible values are:
1: Alaska Native (Aleut, Eskimo, Indian)
2: American Indian (other than Alaska Native)
3: Asian or Pacific Islander
4: Black or African American
5: White
6: Asian
7: Other single race
8: Two or more races
9: Native Hawaiian or Other Pacific Islander
-9: Missing/unknown/not collected/invalid


### ETHNIC: Categorical variable indicating the ethnicity of the individual. Possible values are:
1: Puerto Rican
2: Mexican
3: Cuban or other specific Hispanic
4: Not of Hispanic or Latino origin
5: Hispanic or Latino, specific origin not specified
-9: Missing/unknown/not collected/invalid


### EDUC: Highest level of education completed
1: Less than one school grade, no schooling, nursery school, or kindergarten to Grade 8
2: Grades 9 to 11
3: Grade 12 (or GED)
4: 1-3 years of college, university, or vocational school
5: 4 years of college, university, BA/BS, some postgraduate study, or more
-9: Missing/unknown/not collected/invalid


### EMPLOY: Categorical variable indicating the employment status of the individual. Possible values are:
1: Full-time
2: Part-time
3: Unemployed
4: Not in labor force
-9: Missing/unknown/not collected/invalid


### LIVARAG: Categorical variable indicating the living arrangement of the individual. Possible values are:
1: Homeless
2: Dependent living
3: Independent living
-9: Missing/unknown/not collected/invalid


### PRIMINC: Categorical variable indicating the primary source of income. Possible values are:
1: Wages/salary
2: Public assistance
3: Retirement/pension, disability
4: Other
5: None
-9: Missing/unknown/not collected/invalid


### STFIPS: Census state FIPS code
1: Alabama
2: Alaska
4: Arizona
5: Arkansas
6: California
8: Colorado
9: Connecticut
10: Delaware
11: District of Columbia
12: Florida
13: Georgia
15: Hawaii
17: Illinois
18: Indiana
19: Iowa
20: Kansas
21: Kentucky
22: Louisiana
23: Maine
24: Maryland
25: Massachusetts
26: Michigan
27: Minnesota
28: Mississippi
29: Missouri
30: Montana
31: Nebraska
32: Nevada
33: New Hampshire
34: New Jersey
35: New Mexico
36: New York
37: North Carolina
39: Ohio
40: Oklahoma
42: Pennsylvania
44: Rhode Island
45: South Carolina
46: South Dakota
47: Tennessee
48: Texas
49: Utah
50: Vermont
51: Virginia
54: West Virginia
55: Wisconsin
56: Wyoming
72: Puerto Rico


### REGION: Categorical variable indicating the region of the country where the individual lives. Possible values are:
0: U.S. territories
1: Northeast
2: Midwest
3: South
4: West


### DIVISION: Categorical variable indicating the division within a region where the individual lives. Possible values are:
0: U.S. territories
1: New England
2: Middle Atlantic
3: East North Central
4: West North Central
5: South Atlantic
6: East South Central
7: West South Central
8: Mountain
9: Pacific


### HLTHINS: Categorical variable indicating the health insurance status of the individual. Possible values are:
1: Private insurance, Blue Cross/Blue Shield, HMO
2: Medicaid
3: Medicare, other (e.g. TRICARE, CHAMPUS)
4: None


### SUB1: Categorical variable indicating the primary substance of abuse. Possible values include specific codes for different substances. Some of these codes may include:
1: None
2: Alcohol
3: Cocaine/crack
4: Marijuana/hashish
5: Heroin
6: Non-prescription methadone
7: Other opiates and synthetics
8: PCP
9: Hallucinogens
10: Methamphetamine/speed
11: Other amphetamines
12: Other stimulants
13: Benzodiazepines
14: Other tranquilizers
15: Barbiturates
16: Other sedatives or hypnotics
17: Inhalants
18: Over-the-counter medications
19: Other drugs


## Data Characteristics
Demographics: Includes detailed demographic information such as age, gender, race, ethnicity, education, employment, and marital status.
Geographic Information: Data is categorized by census regions and includes the type of service setting at the treatment facility.
Substance Use Details: Information on the primary, secondary, and tertiary substances of abuse, their frequency of use, and the route of administration.
Treatment History: Data on the number of prior treatment episodes (NOPRIOR), reflecting the history of individuals seeking treatment.


## Columns for regression X - we will use those on sub1 regression:

AGE
GENDER
RACE
ETHNIC
EDUC
EMPLOY
LIVARAG
PRIMINC 
STFIPS
REGION
HLTHINS 

