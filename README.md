# Intelligent Transformer Health Monitoring and Predictive Maintenance System using Machine Learning

## Overview

Distribution transformers are essential components of electrical power distribution networks. Their operating conditions and health directly affect electricity supply reliability, power quality, and maintenance planning.

As an Electrical Power Engineering student at the University of Rwanda, I am exploring how electrical engineering principles, transformer condition indicators, data analysis, and machine learning can be combined to investigate transformer health monitoring and predictive maintenance.

This project focuses primarily on an electrical power engineering challenge: understanding transformer operating conditions and identifying potential signs of abnormal performance. Machine learning will be investigated as a supporting tool for analyzing available data and assisting condition assessment.

The project uses Rwanda’s electricity distribution context as its intended application, with the long-term goal of exploring practical, data-informed approaches to power system reliability and asset maintenance.

## Background and Motivation: Rwanda

Reliable electricity distribution is important for Rwanda’s economic development, industrial growth, and access to essential services. Distribution transformers are critical network assets, making their condition assessment and maintenance important areas of power engineering.

The Rwanda Electricity Distribution Master Plan, published by the Rwanda Energy Group (REG) in June 2022, included an assessment of 6,610 distribution transformers for the week of 27 June to 3 July 2022. The assessment identified 179 heavily loaded transformers and 7 overloaded transformers. The report also discussed transferring or swapping transformer capacity between sites.

These figures describe a historical loading assessment, not current transformer conditions or transformer failure rates. Nevertheless, they illustrate why transformer loading assessment, condition monitoring, and maintenance planning are relevant to electricity distribution in Rwanda.

**Reference:** [Rwanda Electricity Distribution Master Plan — REG, June 2022](https://reg.rw/fileadmin/user_upload/Rwanda_Electricity_Distribution_Master_Plan_-_updated_June_2022.pdf)

## Problem Statement

Distribution transformers operate under varying electrical and environmental conditions. Understanding these conditions is important for identifying abnormal operation, assessing equipment health, and supporting maintenance planning.

Traditional inspection and maintenance approaches can benefit from additional data-driven tools that help engineers analyze measurements and recognize patterns associated with potential problems.

This project investigates how transformer engineering knowledge and data analysis can be combined with machine learning to support condition assessment and maintenance prioritization. The research will examine what can be achieved using suitable available datasets and what further information would be needed before applying the approach to Rwanda’s electricity distribution network.

## Project Aim

To investigate and develop a data-driven approach to distribution transformer health monitoring and predictive maintenance, applying electrical power engineering principles and evaluating machine learning techniques where appropriate.

## Objectives

- Review existing research on distribution transformers, transformer condition monitoring, fault diagnosis, and maintenance practices.
- Identify and assess suitable publicly available transformer datasets.
- Examine relevant transformer operating parameters and condition indicators.
- Perform exploratory data analysis to understand transformer operating patterns and potential abnormal conditions.
- Investigate suitable machine learning methods for anomaly detection or fault classification, depending on the selected dataset.
- Evaluate the methods using appropriate validation techniques and performance metrics.
- Develop a prototype dashboard for visualizing transformer indicators and analytical results.
- Discuss the potential relevance, limitations, and requirements for applying the approach in Rwanda’s electricity distribution context.

## Research Questions

1. Which transformer operating parameters and condition indicators can help assess transformer health?
2. What patterns in available transformer data may indicate abnormal operating conditions or potential faults?
3. How effectively can suitable machine learning methods identify anomalies or classify faults in the selected dataset?
4. How could data-driven transformer condition assessment support maintenance prioritization in Rwanda?
5. What additional data, testing, and engineering validation would be required before applying such an approach in a real distribution network?

## Proposed System

The proposed system will explore the following components:

1. **Transformer data acquisition:** Identify and obtain a suitable public dataset or data for which appropriate access permission has been granted.
2. **Electrical parameter analysis:** Examine available transformer loading, temperature, electrical measurements, or other condition indicators.
3. **Data preparation:** Assess data quality, investigate missing values, and prepare relevant features.
4. **Condition assessment:** Analyze operating patterns and investigate potential indicators of abnormal performance.
5. **Machine learning:** Evaluate appropriate methods for anomaly detection or fault classification when supported by the available data.
6. **Performance evaluation:** Compare model outputs against appropriate reference labels or baseline methods.
7. **Visualization dashboard:** Present relevant transformer indicators and analytical results in an accessible format.
8. **Engineering interpretation:** Discuss the results in the context of transformer operation, maintenance, and electricity distribution reliability.

## Transformer Parameters and Condition Indicators

Depending on the selected dataset, the investigation may include:

- **Loading:** Transformer load levels and variations.
- **Temperature:** Available transformer or oil temperature measurements.
- **Electrical measurements:** Voltage and current measurements, where available.
- **Oil condition:** Relevant oil-related condition indicators, where available.
- **Dissolved Gas Analysis (DGA):** Gas concentrations used in transformer fault diagnosis, if the selected dataset contains them.
- **Historical condition information:** Fault labels, inspection results, or maintenance records, where available and appropriately documented.

The final parameters will depend on the selected dataset. These indicators will be interpreted within their relevant electrical engineering context rather than treated as interchangeable measures of transformer health.

## Data Strategy

The initial stage will focus on identifying suitable datasets and reviewing their sources, documentation, limitations, and relevance to the research questions.

Potential starting points include:

- [DGA Database](https://bmrayan.github.io/dgadb/) — a potential starting point for dissolved gas analysis and transformer fault diagnosis research.
- [IEEE DataPort](https://ieee-dataport.org/) — a research data platform where relevant transformer datasets may be available.
- [Zenodo](https://zenodo.org/) — a research repository that may contain relevant datasets and supporting publications.

These are candidate sources for investigation; the availability and suitability of a particular dataset have not yet been confirmed.

The project will not assume access to confidential operational data from REG or EUCL. Any future use of utility data would require appropriate authorization and compliance with applicable confidentiality and data protection requirements.

If synthetic data is used to test the workflow, it will be explicitly identified as synthetic and will not be presented as real transformer operating data.

## Methodology

### Phase 1: Literature Review

Review technical literature on distribution transformer operation, condition monitoring, fault diagnosis, electrical asset management, and data-driven maintenance.

### Phase 2: Dataset Selection

Identify candidate datasets and assess their relevance, completeness, documentation, and suitability for the selected engineering problem.

### Phase 3: Electrical and Data Analysis

Use Python-based tools to examine available measurements, investigate operating patterns, assess data quality, and identify potentially relevant condition indicators.

### Phase 4: Feature Preparation and Model Development

Prepare appropriate features and select analytical methods based on the engineering objective and characteristics of the data.

Potential methods include:

- Isolation Forest for anomaly detection.
- Random Forest for fault classification.
- Gradient boosting methods where appropriate for classification or prediction.

These methods are candidates rather than predetermined solutions. The final choice will depend on the dataset, available labels, sample size, and research question. Where appropriate, simpler baseline methods will be used for comparison.

### Phase 5: Model Evaluation

Evaluate the selected methods using suitable validation techniques and metrics. Depending on the task, these may include precision, recall, F1-score, confusion matrices, and other relevant measures.

The evaluation will consider class imbalance, data leakage, and the distinction between identifying an existing fault and predicting a future failure.

### Phase 6: Dashboard Development

Develop a prototype dashboard using Streamlit and appropriate visualization tools to display transformer indicators and analytical results.

The dashboard will be a research prototype, not a certified transformer protection system or a replacement for professional engineering assessment.

### Phase 7: Engineering Interpretation and Documentation

Interpret the findings in the context of transformer operation and maintenance. Document the dataset, analytical methods, experimental results, limitations, and recommendations for further research.

## Technologies and Tools

- **Electrical engineering foundation:** Transformer operation, power distribution, condition indicators, and asset maintenance concepts.
- **Programming:** Python.
- **Data analysis:** Pandas and NumPy.
- **Machine learning:** Scikit-learn.
- **Visualization:** Matplotlib and Plotly.
- **Dashboard development:** Streamlit.
- **Development environment:** Jupyter Notebook or Google Colab.
- **Version control:** Git and GitHub.

These tools will support the engineering investigation; their final use will depend on the selected dataset and implementation requirements.

## Expected Deliverables

- A documented and justified transformer dataset.
- An exploratory analysis of relevant transformer parameters and condition indicators.
- A reproducible data preparation and analysis workflow.
- A machine learning prototype appropriate to the selected task.
- Evaluation results using suitable metrics and baseline comparisons, where appropriate.
- A dashboard for visualizing available transformer indicators and analytical outputs.
- A technical report describing the engineering problem, methodology, findings, limitations, and future research directions.

These are planned deliverables. They will be updated as the work progresses and actual results become available.

## Potential Contribution to Rwanda

This project aims to investigate how electrical engineering analysis and data-driven methods could support transformer condition assessment and maintenance planning in Rwanda’s electricity distribution sector.

If supported by reliable data and further validation, such an approach could help engineers investigate abnormal operating conditions, identify assets that may warrant further inspection, and explore more informed maintenance prioritization.

Potential improvements in reliability, maintenance costs, or transformer service life remain hypotheses until demonstrated through appropriate evaluation and real-world validation.

The project is intended to contribute to the exploration of practical engineering solutions for electricity distribution challenges in Rwanda, while recognizing the importance of reliable data, engineering judgment, and collaboration with relevant stakeholders.

## Limitations and Research Integrity

- The quality and representativeness of the selected dataset will influence the findings.
- Results from public datasets may not generalize directly to Rwanda’s electricity distribution network.
- Fault diagnosis is different from predicting future failures or estimating remaining useful life.
- Model outputs will not be presented as verified engineering diagnoses.
- Synthetic data, if used, will be clearly distinguished from real measurements.
- Any performance claims will be based on completed experiments and documented evaluation.
- Deployment in an operational electricity network would require additional validation, engineering review, and appropriate authorization.

## Future Work

Potential future extensions include:

- Investigating authorized transformer operating data from relevant electricity-sector stakeholders.
- Comparing findings across suitable datasets.
- Incorporating time-series analysis if sufficient historical measurements are available.
- Exploring how condition assessment could inform maintenance workflows.
- Evaluating the feasibility of field validation in collaboration with qualified engineers and relevant institutions.

## Author

**Hussein NSANZIMFURA**  
Electrical Power Engineering Student  
University of Rwanda

**Areas of interest:** Electrical Power Systems, Electricity Distribution Networks, Renewable Energy, Transformer Monitoring, and the application of Data Analytics and Machine Learning to Electrical Power Engineering.

## Project Status

**Current stage:** Research planning and dataset selection.

Dataset selection, model development, and experimental evaluation have not yet been completed. This repository will document the project as it progresses, including the data sources, engineering analysis, implementation decisions, results, and limitations.

