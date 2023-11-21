# Hypoglycemia rates & glycemic control after RYGB vs. LSG

Study title: Hypoglycemia rates and glycemic hormonal response after laparoscopic Roux-en-Y gastric bypass versus sleeve gastrectomy. A meta-analysis of comparative studies.

Computational procedure: Variables were divided into primary and secondary, and then analyzed by grouping studies for each outcome.

Outcomes: 
Primary: 
1a. Hypoglycemia rates (OGTT, MMTT, CGM, Questionnaires): RR (relative risk)
1b. Fasting glucose & insulin: MD (mean difference; mg/dl & pmol/l)
1c. Change in glucose & insulin from baseline: MD (mean difference; mg/dl & pmol/l)
1d. OGTT: 1 & 2hr glucose & insulin: MD (mean difference; mg/dl & pmol/l)
1e. OGTT: Change in 1 & 2hr glucose & insulin from baseline: MD (mean difference; mg/dl & pmol/l)

Secondary: 
2a. Male patients: OR (odds ratio)
2b. Change in body weight (BW): MD (mean difference; Kg)
2c. Change in BMI: MD (mean difference; Kg/m^2)
2d. Excess body weight loss (EBWL): MD (mean difference; %)
2e. Change in waist circumference (WC): MD (mean difference; cm)
2f. HbA1c: MD (mean difference; %)
2g. HOMA-IR (insulin resistance score) & change from baseline: MD (mean difference)
2h. Average 10-day hypoglycemic (HG) events: MD (mean difference)
2i. OGTT: Peak glycemia: MD (mean difference; mg/dl)
2j. OGTT: Time to peak glycemia: MD (mean difference; mg/dl)
2k. OGTT: Nadir glycemia: MD (mean difference; mg/dl)
2l. OGTT: Peak - Nadir glycemia range: MD (mean difference; mg/dl)
2m. Postoperative C-peptide levels & change from baseline: MD (mean difference; ng/ml)
2n. 1hr / fasting glucose & insulin ratios (& changes from baseline): MD (mean difference)
2o. 1hr / 2hr glucose & insulin ratios (& changes from baseline): MD (mean difference)


Included items: Individual study data (“.csv” files) & R code (“.txt” files).

Meta-analysis (MA): R code is included for the implementation of a random effects model with the Hartung & Knapp modification for MD, and Mantel–Haenszel method for RR and OR; subgroups: studies published before & after 2018, studies with & without patient matching, studies with & without DM2 patients, stratification of studies according to ROBINS-I tool (Low - Moderate - Serious - Critical).

Meta-regression analysis (MRA): R code is included for the implementation of a random effects model, using the restricted maximum likelihood (REML) estimation; moderators: year of publication, number of quality stars assigned according to the Newcastle - Ottawa Scale (NOS).

Sensitivity analysis (SA): As SA we defined the exclusion of a single study during subgroup analysis (SGA).

Instructions (for the replication of results): Create a desktop folder named “Data” and save the “.csv” files with original data, ensuring to specify the correct absolute/relative paths for your system. The code generates desktop folders with relevant names for storing derived data and plots.
