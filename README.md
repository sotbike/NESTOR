# Trifecta rates & comparative analysis of severe - mild complications, PSM, ischemia duration, and postoperative renal function after RPN/RAPN vs. OPN

Study title: Comparative investigation of therapeutic efficacy in tumor resection between robotic and open partial nephrectomy: A meta-analysis supplemented by time-series and quality-based meta-regression.

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

Meta-analysis (MA): R code is included for the implementation of a random effects model with the Hartung & Knapp modification for MD, and Mantel–Haenszel method for OR; subgroups: trifecta definitions according IT & eGFR, studies published before & after 2018, studies with & without patient matching, mulicenter & single-center studies, stratification of studies according to ROBINS-I tool (Low - Moderate - Serious).

Meta-regression analysis (MRA): R code is included for the implementation of a random effects model, using the restricted maximum likelihood (REML) estimation; moderators: year of publication, number of quality stars assigned according to the Newcastle - Ottawa Scale (NOS).

Sensitivity analysis (SA): As SA we defined the exclusion of studies with a CI95% range greater than 2 SD of the original study set CI95% ranges.

Instructions (for the replication of results): Create a desktop folder named “Data” and save the “.csv” files with original data, ensuring to specify the correct absolute/relative paths for your system. The code generates desktop folders with relevant names for storing derived data and plots.
