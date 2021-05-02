# A case study on ISO 26262 extension for connected driving
This repository presents the results from our case study on i-CAVE architecture for the paper ["A Functional Safety Assessment Method for Cooperative Automotive Architecture"](https://arxiv.org/abs/2104.13729)

## Hazard Analysis and Risk Assessment
[Hazards and associated functions](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/Hazardous%20events.pdf) lists platooning functions from
cooperation perspective and vehicular perspective and associated hazards using guide words: NO, MORE, LESS, PART OF, REVERSE, OTHER THAN, and AS WELL AS.

[Hazardous events](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/Hazardous%20events.pdf) lists hazardous events (from both verhicular and cooperative perspective) derived from the hazards from the prior step. This also includes goals (safety goals) to prevent each hazardous event.

Each hazardous event is associated with a controllability, exposure, and severity which in turn decides the Automotive Safety Integrity Level (ASIL) for that specific event (according to Table 4, Part 3 in [ISO 26262:2018](https://www.iso.org/standard/68385.html)). [ASIL allocation vehicular perspective](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/ASIL%20allocation%20vehicular%20perspective.pdf) and [ASIL allocation cooperative perspective](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/ASIL%20allocation%20cooperative%20perspective.pdf) lists controllability, exposure, and severity scores and resulting ASILs for the safety goal corresponding to each hazardous event from vehicular and cooperarive perspective, respectively.

[Safety goals](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/Safety%20goals.pdf) lists the (aggregated) functional safety goals and associated ASIL, where each (aggregated) functional safety goal is the combination of similar safety goals from the previous step and the corresponding ASIL is the highest of all the aggregated safety goals.

## Safety Analysis
[FSRs grouped on functional architecture component](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/FSRs%20grouped%20on%20functional%20architecture%20component.pdf) lists the Functional Safety Requirements (FSRs) generated from the functional safety goals of previous step using fault tree analysis. These FSRs are grouped based on which functional architecture component they are associated with. [FSRs and applicable safety tactics](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/FSRs%20grouped%20on%20functional%20architecture%20component.pdf) shows which safety goals each FSR is derived from.


## Safety Tactics allocation
[FSRs and applicable safety tactics](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/FSRs%20grouped%20on%20functional%20architecture%20component.pdf) lists safety tactics that can be used to achieve each FSR.

[FSRs and associated safety patterns (FSRs unfulfilled)](https://github.com/SangeethNila/casestudy_ISO26262_extension_connected_driving/blob/main/FSRs%20and%20associated%20safety%20patterns%20(FSRs%20unfulfilled).pdf) presents the result of applying proposed method ([Section 3.2 Check fulfillment of FSR](https://arxiv.org/abs/2104.13729)) on i-CAVE software architecture. Specifically, those FSRs that are found not to be fulfilled in the architecture. The FSRs, that are found to be fulfilled are presented in [Table 2](https://arxiv.org/abs/2104.13729).



## How can I cite this work?
If you find this case study useful and want to use it in your work, please cite the following paper: [A Functional Safety Assessment Method for Cooperative Automotive Architecture](https://arxiv.org/abs/2104.13729)
```
@article{kochanthara21functional,
  author = {Kochanthara, Sangeeth and Rood, Niels and Khabbaz Saberi, Arash and Cleophas, Loek and Dajsuren, Yanja and van den Brand, Mark},
  title = {A Functional Safety Assessment Method for Cooperative Automotive Architecture},
  journal = {Journal of Systems and Software},
  year = {2021},
  publisher = {Elsevier}
}
```




