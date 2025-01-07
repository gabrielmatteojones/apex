---
title: "Advanced Duplicate Detection: North Carolina Voter Registration Database Analysis"
layout: post
author: RootSquare
category: Data Analysis
---


At RootSquare.io, we specialize in advanced data cleansing solutions specifically designed for healthcare organizations. Our proprietary technology excels at identifying and resolving duplicate patient records within person demographic data, even in nuanced cases arising from marriage/separation. Remarkably, our solution can even distinguish twins with exceptional accuracy.
    
     

To demonstrate the effectiveness of our solution in a real-world scenario, we applied it to the **North Carolina Voter Registration Database**. This publicly available dataset allowed us to rigorously test our methodologies for identifying duplicate persons. Our solution successfully identified **2,607 potential duplicate pairs** within the dataset. As part of our solution, we then classified them into the following categories:

- Standard duplicates (same individuals with multiple records)  - **SD**
- Duplicates caused by **marriage/separation**  - **MS**
- Cases involving **Multible births or family members**  - **T**
- Non duplicates - **ND**

We prioritize accuracy to ensure our solution flags true duplicates while minimizing the risk of incorrectly identifying separate individuals. 
<br>
This minimizes the need for manual review and ensures data integrity.

**Our solution depicts high accuracy for each category 89%, 91%, 98%, and 96%, respectively.** 

#### *“The average duplicate rate within healthcare organizations is 18%”- [Verato](https://verato.com/blog/three-hidden-costs-of-duplicate-records/#:~:text=According%20to%20a%20recent%20Black,fall%20into%20three%20primary%20categories.)*

Our solution can deliver a powerful impact on healthcare organizations by:

1.  **Protecting Patient Safety:** By eliminating duplicate records, we ensure that healthcare professionals have access to accurate and complete patient information, minimizing the risk of adverse events.
2.  **Optimizing Operational Efficiency:** Our automated solution streamlines data management processes, freeing up valuable time and resources for healthcare staff.
3.  **Reducing Healthcare Costs:** By minimizing errors, reducing manual effort, and improving resource allocation, our solution contributes to significant cost savings.
4.  **Empowering Data-Driven Insights:** Clean and reliable data empowers healthcare organizations to conduct more effective analytics and research, driving innovation and improving patient care.

The result is a more accurate, efficient, and cost-effective healthcare system, ultimately leading to better patient outcomes and an enhanced quality of life for both patients and healthcare providers.

## Technical Analysis Overview

### 0. Data

The data for this analysis originated from the North Carolina Voter Registration Database, available at [North Carolina State Board of Elections](https://www.ncsbe.gov/results-data/voter-registration-data).
The total amount of active records analysed was **6,455,829**. 

### 1. Types of Duplicates  

#### **Figure: Bar chart showing types of duplicates**  
*Bar chart visualizing the distribution of standard duplicates, marriage/separation duplicates, and twins.*

![Analysis Bar Chart](/dup_figs_maps/plot_dups_types.png "Bar Chart of Duplicate Types")


### 2. Standard Duplicates (same individuals with multiple records)  

- *Interactive map showing the geographical distribution of duplicates.*  

<div style="position: relative; width: 100%; padding-bottom: 56.25%;">
    <iframe 
        src="/dup_figs_maps/map_standard_dups.html" 
        style="position: absolute; width: 100%; height: 100%; border: none;">
    </iframe>
</div>

- **Demographics Subplots**: *Figure illustrating age, race, party, voter registration status, and gender distributions among duplicates.*

![population characteristics](/dup_figs_maps/plot_stand_dups_stats.png)

- **Findings**:  
  - Highest sex rate: Female-Female
  - Higest race rate: W, B (White, Black) 
  - Highest party rate: UNA-UNA, Dem-Dem (Democrats)  



### 3. Duplicates from Marriage/Separation  

- *Interactive map showing the geographical distribution of duplicates.*  

<div style="position: relative; width: 100%; padding-bottom: 56.25%;">
    <iframe 
        src="/dup_figs_maps/map_married_dups.html" 
        style="position: absolute; width: 100%; height: 100%; border: none;">
    </iframe>
</div>

- **Demographics Subplots**: *Figure illustrating age, race, party, voter registration status, and gender distributions among duplicates.*

![population characteristics](/dup_figs_maps/plot_married_dups_stats.png)

- **Findings**:  
  - Highest sex rate: Female-Female
  - Higest race rate: W, B (White, Black) 
  - Highest party rate: Dem-Dem, UNA-UNA (Democrats)   
  


### 4. Twins  

- *Interactive map showing the geographical distribution of twins.*  

<div style="position: relative; width: 100%; padding-bottom: 56.25%;">
    <iframe 
        src="/dup_figs_maps/map_twins.html" 
        style="position: absolute; width: 100%; height: 100%; border: none;">
    </iframe>
</div>

- **Demographics Subplots**: *Figure illustrating age, race, party, voter registration status, and gender distributions among duplicates.*

![population characteristics](/dup_figs_maps/plot_twins_stats.png)

- **Findings**:  
  - Highest sex rate: Female-Female, Male-Male
  - Higest race rate: B (Black) 
  - Highest party rate: Dem-Dem, UNA-UNA (Democrats) 
  - Highest age rate: 18-32 years old

**References:**  
**Studies aligning with race and sex distribution findings for twins:**  
- The twin birth rate in the United States in 2022 was 31.2 twins per 1,000 births. The twin birth rate rose for Black women from 40.6 in 2021 to 41.4 in 2022.  The twin birth rate remained essentially unchanged for White women (32.5 to 32.6) and Hispanic women (24.2 to 24.5). ( National Vital Statistics Reports - Volume 73, Number 2 April 4, 2024 )
- Data births of twins peakes aroud 2000s as depicted by the age of [twins duplicates](https://www.cdc.gov/nchs/data/databriefs/db351-h.pdf)
- The higher proportion of female twins compared to male twins is influenced by several biological factors:

    1. **In-Utero Survival Rates**: Male fetuses generally have higher in-utero mortality rates than female fetuses. This disparity is more pronounced in twin pregnancies, leading to a higher proportion of surviving female twins. [Learn more on Wikipedia](https://en.wikipedia.org/wiki/Twin).

    2. **Sex Ratio at Birth**: While the natural sex ratio at birth slightly favors males (approximately 105 males for every 100 females), the increased male fetal mortality in twin pregnancies results in a more balanced or slightly female-skewed sex ratio among twins. [Learn more on Wikipedia](https://en.wikipedia.org/wiki/Twin).




Rootsquare.io’s solution demonstrates unparalleled accuracy in identifying duplicates across diverse datasets. This analysis highlights the potential of our tools to streamline database management and improve data integrity.

For more information about our services, visit **[Rootsquare.io](https://rootsquare.io)** or contact us directly.  
