# Analysis

FREAS supports analysis of BPMN4FRSS models to determine their correctness, give feedback to the modeller, and, most importantly, allow for assessment of the forensic-ready software system capabilities.

## Semantic Rules Analysis

Verifies if the provided model is in accordance with BPMN4FRSS semantic rules. Thus, the model is checked to determine whether the introduced BPMN4FRSS constructs make sense and can correctly describe the state of forensic readiness within the system. 

If the model violates any of the rules, the tool displays an indication of which part of the model is violating a rule. Furthermore, it provides an **Error** message that details the problem and can help the modeller to fix the issue.

## Semantic Hints Analysis

Provides recommendations for improving the model. The model is checked to uncover potential problems that could negatively affect the system's forensic readiness capabilities. However, they are not affecting the model's validity.

If the model violates any of the rules, the tool displays an indication of which part of the model is violating a rule. Furthermore, it provides an **Warnings** message that details the problem and can help the modeller to improve the model. Compliance with these rules is highly recommended, as their violation can indicate potential weaknesses

## Evidence Quality Analysis

Checks whether the employed forensic-ready controls are sufficient to yield reliable and relevant potential evidence in case of an incident that compromises concrete **Data Store** or a **Flow Object** (Task or Event). To simulate an incident, the user must mark a corresponding element from the model as compromised, i.e., select the **id** of the element in the sidebar. In both cases, as a result, analysis marks all Data Store elements that contain potential evidence connected to the incident. Stored potential evidence can hold information to help detect the inconsistency between the data.