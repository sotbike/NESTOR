# Trifecta rates & comparative analysis of severe - mild complications, PSM, ischemia duration, and postoperative renal function after RPN/RAPN vs. OPN

Study title: Differential Therapeutic Efficacy of Robotic vs. Open Partial Nephrectomy in Tumor Resection: A Meta-Analysis with Stratified Multidimensional Meta-Regression.
Computational procedure: Variables were divided into primary and secondary, and then analyzed by grouping studies for each outcome.

Outcomes: 

Primary: 
1. Trifecta rates (concomitant achievement of no complications, negative surgical margins and IT < 20 min or ΔeGFR < 10%): OR (odds ratio)

Secondary: 
2a. Major complication rates (defined as Clavien - Dindo ≥ III): OR (odds ratio)
2b. Minor complication rates (defined as Clavien - Dindo ≤ II): OR (odds ratio)
2c. Positive surgical margin (PSM) rates: OR (odds ratio)
2d. Ischemia time (IT): MD (mean difference; min)
2e. Change from baseline in eGFR (ΔeGFR): MD (mean difference; ml/min/1.73m^2)
2f. Change from baseline in serum creatinine levels (ΔCreatinine): MD (mean difference; mg/dl)


Included items: Individual study data (“.csv” files) & R code (“.txt” files).

Meta-analysis (MA): R code is included for the implementation of a random effects model with the Hartung & Knapp modification for mean differences (MD), and the Mantel–Haenszel method for odds ratios (OR). Subgroup analyses were conducted based on: trifecta definitions according to ischemia time (IT) and estimated glomerular filtration rate (eGFR), studies published before and after 2018, studies with and without patient matching, multicenter versus single-center studies, and stratification according to the ROBINS-I tool (Low – Moderate – Serious). Publication bias was assessed using Egger’s test, while small-study effects were examined according to the method proposed by Schwarzer.

Meta-regression analysis (MRA): R code is included for the implementation of a random effects model using the restricted maximum likelihood (REML) estimation method. The model incorporates the following moderators: year of publication, number of quality stars assigned according to the Newcastle-Ottawa Scale (NOS), mean tumor size, and average R.E.N.A.L. score. Internal validation was performed using Cook’s distance analysis (threshold = 1) to identify influential studies.

Sensitivity analysis (SA): The first level of the SA includes studies with increased precision in their reported outcomes (exclusion of studies with a 95% confidence interval range greater than 2 standard deviations from the original study set’s 95% CI ranges), whereas the second level of the SA includes studies in which the compared patient populations do not differ in baseline characteristics.

Instructions (for the replication of results): Create a desktop folder named “Data” and save the “.csv” files with original data, ensuring to specify the correct absolute/relative paths for your system. The code generates desktop folders with relevant names for storing derived data and plots.
