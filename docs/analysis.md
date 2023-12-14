# Analysis

FREAS supports analysis of BPMN4FRSS models to determine their correctness, give feedback to the modeller, and, most importantly, allow for assessment of the forensic-ready software system capabilities.

## Semantic Rules Analysis

Verifies if the provided model is in accordance with BPMN4FRSS semantic rules. Thus, the model is checked to determine whether the introduced BPMN4FRSS constructs make sense and can correctly describe the state of forensic readiness within the system. 

If the model violates any of the rules, the tool displays an indication of which part of the model is violating a rule. Furthermore, it provides an **Error** message that details the problem and can help the modeller to fix the issue.

## Semantic Hints Analysis

Provides recommendations for improving the model. The model is checked to uncover potential problems that could negatively affect the system's forensic readiness capabilities. However, they are not affecting the model's validity.

If the model violates any of the rules, the tool displays an indication of which part of the model is violating a rule. Furthermore, it provides an **Warnings** message that details the problem and can help the modeller to improve the model. Compliance with these rules is highly recommended, as their violation can indicate potential weaknesses

## Evidence Quality Analysis

This analysis queries the model to determine whether the employed forensic-ready controls are sufficient to yield reliable and relevant potential evidence in case of a compromise. This means asking if there is potential evidence within the system that would show that another piece of potential evidence is falsified due to the compromise. The analyst selects a concrete **Data Store** (Data Store Reference) or a **Flow Object** (Task or Event) as compromised to mark an IS Asset that was compromised in an incident. Such IS Asset is then assumed to produce falsified potential evidence.

The analyst selects the **id** of the desired element in the sidebar to mark the compromised IS Asset. As a result, the analysis marks all Data Stores that contain reliable potential evidence connected to the incident. The stored potential evidence in those Data Stores can hold information to help detect the inconsistency between the data.