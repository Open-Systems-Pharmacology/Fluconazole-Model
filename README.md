# Fluconazole-Model
Whole-body PBPK model of fluconazole.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4e/Fluconazole_skeletal_formula.svg/512px-Fluconazole_skeletal_formula.svg.png" alt="File:Fluconazole skeletal formula.svg" style="zoom:50%;" />





This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation-plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found [here](../../releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found [here](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**



This fluconazole model is intended to be used as perpetrator drug in CYP3A4-mediated drug-drug interactions (DDI).

This whole-body PBPK model of fluconazole has been developed using published pharmacokinetic clinical data by Palkama et al. 1998 [[1](#references)], Ripa et al. 1993 [[2](#references)], Shiba et al. 1990 [[3](#references)], Ahonen et al. 1997 [[4](#references)], Brammer et al. 1990 [[5](#references)], Brammer et al. 1991 [[6](#references)], Thorpe et al. 1990 [[7](#references)] and Varhe et al. 1996 [[8](#references)]. 
The model has then been evaluated simulating clinical studies and comparing with respective observed data. 

The presented model includes the following features:

- metabolism by UGT2B7,
- inhibition of CYP3A4,
- renal clearance by glomerular filtration,
- oral absorption with dissolution rate assigned to the Weibull function for low, medium and high doses.


## Code of conduct

Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution

We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License

The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References

[1] [Palkama VJ, Isohanni MH, Neuvonen PJ, Olkkola KT. The effect of intravenous and oral fluconazole on the pharmacokinetics and pharmacodynamics of intravenous alfentanil. Anesth Analg. 1998 Jul;87(1):190-4.](https://journals.lww.com/anesthesia-analgesia/Fulltext/1998/07000/The_Effect_of_Intravenous_and_Oral_Fluconazole_on.39.aspx)

[2] [Ripa S, Ferrante L, Prenna M. Pharmacokinetics of fluconazole in normal volunteers. Chemotherapy. 1993;39(1):6-12.](https://doi.org/10.1159/000238967)

[3]  [Shiba K, Saito A, Miyahara T. Safety and pharmacokinetics of single oral and intravenous doses of fluconazole in healthy subjects. Clin Ther. 1990 May-Jun;12(3):206-15.](https://pubmed.ncbi.nlm.nih.gov/2379224/)

[4] [Ahonen J, Olkkola KT, Neuvonen PJ. Effect of route of administration of fluconazole on the interaction between fluconazole and midazolam. Eur J Clin Pharmacol. 1997;51(5):415-9.](https://link.springer.com/article/10.1007/s002280050223)

[5] [Brammer KW, Farrow PR, Faulkner JK. Pharmacokinetics and tissue penetration of fluconazole in humans. Rev Infect Dis. 1990 Mar-Apr;12 Suppl 3:S318-26.](https://academic.oup.com/cid/article-abstract/12/Supplement_3/S318/300865?redirectedFrom=fulltext)

[6] [Brammer KW, Coakley AJ, Jezequel SG, Tarbit MH. The disposition and metabolism of [14C]fluconazole in humans. Drug Metab Dispos. 1991 Jul-Aug;19(4):764-7.](https://pubmed.ncbi.nlm.nih.gov/1680653/)

[7] [Thorpe JE, Baker N, Bromet-Petit M. Effect of oral antacid administration on the pharmacokinetics of oral fluconazole. Antimicrob Agents Chemother. 1990 Oct;34(10):2032-3.]( https://doi.org/10.1128/AAC.34.10.2032)

[8] [Varhe A, Olkkola KT, Neuvonen PJ. Effect of fluconazole dose on the extent of fluconazole-triazolam interaction. Br J Clin Pharmacol. 1996 Oct;42(4):465-70.](https://pubmed.ncbi.nlm.nih.gov/8904618/)

