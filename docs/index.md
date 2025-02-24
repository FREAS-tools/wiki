# Quick Guide

FREAS is a modeling and analysis tool for forensic-ready software systems. The tool allows users to import or model business processes using the BPMN for Forensic-Ready Systems (BPMN4FRSS) notation. On the provided BPMN4FRSS model, users can run different types of analysis to evaluate the extent to which the modeled system complies with forensic readiness requirements. Furthermore, users can assess the system's ability to provide evidence with high evidentiary value in case of an incident. 

As a result, the tool allows users to inspect the possible model insufficiencies and offers hints to remedy the issue.

FREAS can be deployed locally using [docker compose](https://raw.githubusercontent.com/FREAS-tools/freas-demo/main/docker-compose.yml).

## Example

Example models are available on [GitHub](https://github.com/FREAS-tools/freas-demo/).

## Modeling

FREAS allows for the graphical modelling of BPMN4FRSS diagrams, which can be exported as models. These models can then be fed into the analysis module.

The toolbox on the left contains BPMN and BPMN4FRSS elements that can be placed into the canvas. Then, the elements can be modified using a contextual pad (available when selected) or the properties panel on the right. Connections between the elements can be drawn using the tools from the contextual pad. Properties of the element can be edited using the properties panel.

Please see the [Modelling](modelling.md) for further details on the tool and [Model Creation](BPMN4FRSS/model_creation.md) for details on BPMN4FRSS elements and semantics.

## Analysis

Clicking on the "Show validation" displays a right sidebar where the analysis type can be specified and validation executed. The validation result is shown in the form of a message next to the corresponding elements.

Three types of analysis are available:

* Semantic Rules Analysis
* Semantic Hints Analysis
* Evidence Quality Analysis

Please see the [Analysis](analysis.md) for further details on the available analyses.