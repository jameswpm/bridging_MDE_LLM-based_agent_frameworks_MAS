# Bridging MDE and LLM-based Agent Frameworks for Multi-Agent Systems: A Quasi-Systematic Review and Metamodel

This repository contains artifacts for the paper *"Bridging MDE and LLM-based Agent Frameworks for Multi-Agent Systems: A Quasi-Systematic Review and Metamodel"* accepted for publication and presentation to the **14th International Conference on Model-Based Software and Systems Engineering (MODELSWARD 2026)**.

## Overview

This repository provides the research artifacts for the presented paper, including the metamodel project and supplementary material for validation and potential reproduction of the results.

## Project Description

This research systematically analyzes the landscape of AI agent frameworks to identify common patterns, terminologies, and concepts. The study resulted in a formal metamodel that can serve as a foundation for understanding, comparing, and potentially standardizing agent framework architectures.

## Technical Implementation

* **Eclipse EMF**: Used for metamodel definition and tooling.

## Usage

All the artifacts mentioned in the paper are ready to be used. Below are the instructions to import this project into your own Eclipse environment and (re-)generate all artifacts, as well as use the collected data for reproduction, automation, and/or validation.

### Running the Eclipse project for metamodel creation

#### Prerequisites

Before running this project, make sure you have:

* **Java Development Kit (JDK 8 or later)** installed and configured.
* **Eclipse Modeling Tools** (latest stable release).
* **Emfatic plugin** installed in Eclipse (via *Help → Install New Software...*).

#### Running the project

1. **Import the project**: Use *File → Import → Existing Projects into Workspace* and select the root folder of this project.
2. **Open the Emfatic file**: Locate the `.emf` file and open it using the Emfatic editor (you may optionally include/exclude elements).
3. **Generate the Ecore model**: Right-click on the `.emf` file and choose *Generate Ecore Model*. This will produce the `.ecore` definition.

After this, the metamodel is ready to be used in your EMF-based applications or tools.

## Data Files

The folder `data` is not part of the Eclipse project. It contains supplementary files used for validation of the collected data.

### Framework Evaluation Data

* **FULL_LIST_FRAMEWORKS_NOTES.csv**: Complete evaluation of 75 frameworks considering the defined criteria (see Table 1 in the paper).
* **TERMINOLOGY.csv**: Collected terminology with definitions, frequency analysis, and importance scoring.
* **FRAMEWORKS_AND_TERMINOLOGY.xlsx**: Combined data from the two CSV files, with improved formatting for visualization.
* **action_phrases.md**: A set of phrases elaborated to help in the metamodel definition (see Section 4 of the paper).

## Repository Structure

```
├── data/                                 # Research supplementary data
│   ├── FULL_LIST_FRAMEWORKS_NOTES.csv     # Full list of 75 frameworks analyzed (CSV)
│   ├── TERMINOLOGY.csv                    # Terminology definitions and scoring (CSV)
│   ├── FRAMEWORKS_AND_TERMINOLOGY.xlsx    # Combined list and terminology in Excel format
│   └── action_phrases.md                  # Relationship definitions between concepts as action phrases
├── figures/                              # Generated diagrams and visualizations
│   ├── communication_class_diagram.*      # Communication package
│   └── construction_class_diagram.*       # Construction package
├── agent_frameworks.ecore                # Eclipse EMF metamodel definition
├── agent_frameworks.emf                  # Textual metamodel representation using Emfatic
├── agent_frameworks.genmodel             # EMF code generation model
└── agent_frameworks.aird                 # Sirius modeling project file for diagrams generation
```
**Note: ** `figures` contain the diagram in diffeent file formats to allow proper navigation and high resolution.

## Contact

James Pontes Miranda
CEA-List, Paris-Saclay, France
DRT / LIST
james.pontesmiranda@cea.fr

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{Miranda2026_MDE_LLM_Agents,
  author    = {Miranda, James Pontes and Radermacher, Ansgar and Baligand, Fabien and Bonnail, Julie and G{\'e}rard, S{\'e}bastien and Bannerot, Pascal and Del Fabro, Marcos Didonet},
  title     = {Bridging {MDE} and {LLM}-{Based} {Agent} {Frameworks} for {Multi}-{Agent} {Systems}: {A} {Quasi}-{Systematic} {Review} and {Metamodel}},
  booktitle = {Proceedings of the 14th International Conference on Model-Based Software and Systems Engineering},
  year      = {2026},
  pages     = {33--44},
  isbn      = {978-989-758-798-6},
  issn      = {2184-4348}
}
```

---

**Note**: This repository contains research artifacts from an academic study. The metamodel and analysis are intended for research and educational purposes.
