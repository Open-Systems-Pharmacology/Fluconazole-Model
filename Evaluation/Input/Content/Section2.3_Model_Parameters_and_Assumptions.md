### 2.3.1 Absorption

The parameter value for  `Specific intestinal permeability`  was used as in GastroPlus. Although, the permeability didn't seem to be the rate-limiting step  in oral absorption as this parameter could not be identified when attempting to estimate a value using Parameter Identification. The default solubility was assumed to be the measured value in phosphate buffer (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data))

The dissolution of capsules/tablets (not always specified in the literature which formulation for oral administration was used) were implemented via empirical Weibull dissolution. A different Weibull function was used for different dose categories, low, medium high and high dose to distinguish the dissolution time across the dose range; see results of optimization in [Section 2.3.4](#234-automated-parameter-identification).

### 2.3.2 Distribution

Fluconazole has a low protein bound (approx. 11 %) fraction in plasma (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)). A value of 89% was used in this PBPK model for `Fraction unbound (plasma, reference value)`. The major binding partner was set to alpha1- acid glycoprotein(see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

An important parameter influencing the resulting volume of distribution is lipophilicity. The reported experimental logP values are in the range of 0.5-1.0 (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)) which served as a starting value. Finally, the model parameters `Lipophilicity` was optimized to match best clinical data (see also [Section 2.3.4](#234-automated-parameter-identification)).

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard`.

### 2.3.3 Metabolism and Elimination

One metabolic pathway was implement into the model via first order kinetics 

* UGT2B7

The UGT2B7 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). Absolute tissue-specific expressions were obtained by considering the respective absolute concentration in the liver. The `Specific clearance ` of fluconazole accounted by UGT2B7 was identified to best describe observed clinical data after intravenous administration (see [Section 2.3.4](#234-automated-parameter-identification)).

Additionally, renal clearance (which is the main elimination process for fluconazole) assumed to be mainly driven by glomerular filtration was implemented. The `GFR fraction` was identified to best describe the observed fraction of unchanged fluconazole that was renally excreted (see [Section 2.3.4](#234-automated-parameter-identification)).

### 2.3.4 Automated Parameter Identification

This is the result of the final parameter identification for the intravenous model:

| Model Parameter                | Optimized Value | Unit      |
| ------------------------------ | --------------- | --------- |
| `Lipophilicity`                | 0.83            | Log Units |
| `GFR fraction`                 | 0.14            |           |
| `Specific clearance ` (UGT2B7) | 1.85E-3         | 1/min     |



This is the result of the final parameter identification for the dissolution parameters of a oral administered fluconazole:

| Model Parameter                                     | Optimized Value | Unit |
| --------------------------------------------------- | --------------- | ---- |
| `Dissolution time (50% dissolved) high dose`        | 105.81          | min  |
| `Dissolution time (50% dissolved) medium high dose` | 75.14           | min  |
| `Dissolution time (50% dissolved) low dose`         | 33.40           | min  |
| `Dissolution shape`                                 | 2.14            |      |

