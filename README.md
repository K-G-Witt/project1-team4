# Introduction
The source data collected for this project was produced by Open Sourcing Mental Health, previously OSMI, and was titled Mental Health in Tech. Our team chose a topic that we found interesting and relevant, and the analysis provided some unexpected results.

# Background 
Tech workers experience precarious employment, unpredictable working hours, sedentary, and often socially isolating working conditions. Research on psychosocial working conditions suggests that these factors are likely to have significant impacts on workers' mental and physical health. Increasingly, research is suggesting that workplace cultures that encourage workers to disclose their mental health issues to colleagues and supervisors may improve the likelihood that workers will disclose mental health conditions, leading to better long-term outcomes for tech workers. 

The COVID-19 pandemic has led to significant global casualties and long-term complications for individuals who have recovered from the viral infection. Since the initial confirmation of diagnoses, interdisciplinary researchers worldwide have collaborated on disease precautions and treatments for viral infections. However, there has been limited research on the mental health of the public during the COVID-19 period.

# Purpose
The aims of this project are therefore to explore the factors that impact on tech workers mental health over two observation periods, before the COVID-19 pandemic (2014) compared with during the COVID-19 pandemic (2020-2022). We looked at several key indicators including the use of wellness programs within the workplace, how comfortable employees were with reporting the state of their mental health to co-workers and their supervisors. We also looked at whether working remotely had any impact on mental health in this sector. To gain accurate insights, we used data collected globally, over a time period of several years.

# The research questions
1. What is the self-reported prevalence of mental health conditions amongst tech industry workers.
2. How does this compare within different countries?
3. What is the proportion of tech employers that offer wellness programs?
4. Does the prevalence of self reported mental health conditons vary between remote vs. office-based workers?
5. Does the prevalence of self reported mental health conditons vary between a given family history of mental illness?
6. How likely are those with self reported mental health conditions likely to disclose to supervisors verses co-workers?
7. How likely are those with self reported mental health conditions likely to disclose to co-workers?

# Methods
1. Initial import from .csv file into Pandas Data frame for each individual year.
2. Each specific column was selected via filter which would then answer our hypothesis questions. 
3. 2014 data was completely different in data structure, so this was analysed separately. 1259 respondents were in this dataset.
4. To guarantee that the sample size is sufficient to yield adequate statistical power, we merged 2020, 2021 and 2022 survey data. This merged dataset had initially 475 respondents, but this was filtered down to “current” Tech Workers which reduced down to 255 responses.
5. Matplotlib was used to establish a proportion based approach and was utilized to visualize the distribution of participants' responses for all research questions. Additionally, for survey questions with identical answer options, supplementary chi-square tests were conducted to assess changes in distribution.

# Results
- Slide 5 - There was no significant difference found between the pre-pandemic and post-pandemic period when it came to self-reporting of mental health conditions with just over half of all particpants reporting mental health conditions during both periods.
- Slide 7 & 8 - The USA was the largest contributor of respondents followed by the U.K. A combined total of 38 countries participated in the survey. 
- Slide 10 - There was a significant increase of 24.2% for tech companies providing mental health wellness programs between 2014 and 2022. This could be attributed to a positive outcome as a result of the pandemic and or a better recognition or understanding of mental health issues during this period.
- Slide 12 -  Comparing office based workers to remote workers was conducted on the 2014 dataset only. It was found that tech workers working in an office environment were more than twice as likely to identify as having mental health issues when compared to their counterparts who work remotely. 
- Slide 14 - Results showed that the pandemic didn’t have a significant impact on the percentage of tech workers with mental health issues where there was a family history of mental health issues. For 2014 the number of workers who reported "yes" was 57.3% and this dropped slightly to 56.0% during 2020-2022.
- Slide 16 -  There was zero change between pre and post-pandemic surveys for workers willingness to disclose their mental health issues to a supervisor, with only 39.2% willing to do so. 
- Slide 18 - There was however an increase in the percentage of employees willing to talk to co-workers, which increased from 20.1% to 36.8% over the period.

# Limitations
1. Divergence in questions and response options employed in surveys before and after COVID, making it inappropriate to utilize the chi-square test for comparing distribution variance.
2. The way mental health among tech workers is determined relies on whether they sought help from a medical professional. However, COVID-19-related restrictions on selective medical services might introduce bias against those genuinely experiencing mental health issues.
3. Majority of respondents from USA with very different healthcare model to, e.g., AUS
4. Changes may also reflect processes, such as greater awareness of programs and policy changes, rather than being wholly attributable to COVID-19

# Future recommendations
1. Time series analysis could help to identify whether COVID-19, or another factor (e.g., local industrial policies), influences the proportions of tech workers reporting MH issues.
2. Using a dimensional approach to determine MH issues (e.g., scores on a MH screener) would provide greater statistical power.
3. Development of a standardised data dictionary for comparison from previous years.  



## Usage Instructions
### Analysis:
The script, titled **rcl_file**, will generate all the analyses used in this project.

### Visualisations:
The script, titled **rcl_file**, will generate all the visualisations used in this project. All visualisation exhibits used in this project are also saved, in .png format, to a subfolder titled **Exhibits**.

### Datasets:
Mental Health in the Tech Workplace. Resources, including the raw .csv data files used in this project, are available from: https://osmhhelp.org/research.html (accessed 2 April 2024).

## Installation and Run Instructions
### Data files:
The subfolder, titled **Resources**, contains the following four raw datafiles, saved in .csv format, needed for this project:
1. OSMI 2014 Mental Health in Tech Survey Results
2. OSMI 2020 Mental Health in Tech Survey Results
3. OSMI 2021 Mental Health in Tech Survey Results
4. OSMI 2022 Mental Health in Tech Survey Results

## Credits
This code was compiled and written by James Radford, Katrina Witt, Joyce Xu, and Erin Nicol for Project 1 in the 2024 Data Analytics Boot Camp hosted by Monash University. 

## Additional credits are declared below:

### Resetting index to column
https://pandas.pydata.org/docs/reference/api/pandas.Series.reset_index.html#pandas.Series.reset_index (accessed 10 April 2024).

### Scipy chi2_contingency test for independence:
https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chi2_contingency.html (accessed 11 April 2024).

### Using pandas series.map() function to harmonise response options between surveys:
https://pandas.pydata.org/docs/reference/api/pandas.Series.map.html#pandas.Series.map (accessed 10 April 2024).

### Reference material
Padma, V., Anand, N. N., Gurukul, S. M., Javid, S. M., Prasad, A., & Arun, S. (2015). Health problems and stress in Information Technology and Business Process Outsourcing employees. Journal of pharmacy & bioallied sciences, 7(Suppl 1), S9–S13. https://doi.org/10.4103/0975-7406.155764



