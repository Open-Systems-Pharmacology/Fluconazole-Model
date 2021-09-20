The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](#5-references)). Relevant information on anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([Willmann 2007](#5-references)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([PK-Sim Ontogeny Database Version 7.3](#5-references)) or otherwise referenced for the specific process.

A mean model was built based on clinical data from studies with intravenous administration of fluconazole by Palkama et al. 1998 ([Palkama 1998](#5-references)), Ripa et al. 1993 ([Ripa 1993](#5-references)) and Shiba et al. 1990 ([Shiba 1990](#5-references)). The studies conducted by Palkama et al. and Ripa et al. reported plasma concentrations of fluconazole and the study by Shiba reported fraction of unchanged fluconazole excreted to urine in addition to plasma concentrations.  The mean PBPK model was developed using a typical male European individual. The relative tissue-specific expressions of enzymes predominantly being involved in the metabolism of fluconazole (UGT2B7) were considered ([Meyer 2012](#5-references)).

A specific set of parameters (see below) was optimized to describe the distribution of fluconazole after intravenous administration using the Parameter Identification module provided in PK-Sim®. Structural model selection was mainly guided by visual inspection and total error of the resulting description of data, 95% confidence interval of the identified parameter values and biological plausibility.

Once the appropriate structural model was identified for the intravenous administration, the model was verified by simulating other clinical studies reporting pharmacokinetic concentration-time profiles after intravenous administration of fluconazole. 

Thereafter additional parameters for oral administration of non-dissolved formulations (i.e. capsules) were identified. Administered doses of fluconazole were ranging from single dose of 25 mg to multiple dosing of 400 mg, why the applied Weibull function to describe the dissolution of fluconazole were divided into low, medium and high dose. The dissolution shape were kept between the doses while the dissolution time were separated. 

The model was then verified by simulating further clinical studies reporting pharmacokinetic concentration-time profiles after oral administration of fluconazole.

Details about input data (physicochemical, *in vitro* and clinical) can be found in [Section 2.2](#22-data-used).

Details about the structural model and its parameters can be found in [Section 2.3](#23-model-parameters-and-assumptions).



