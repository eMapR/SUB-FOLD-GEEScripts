# SUB-FOLD-GEEScripts

This repository holds the instructions on how to add the Google Earth Engine (GEE) repository to your GEE account. 

# Forest Disturbance Ensemble – GEE Scripts

This repository links to a collection of Google Earth Engine (GEE) scripts for collecting forest change products, creating reference data for evaluating many products at once, and generating forest disturbance map products.  

---

## Documentation

- **[Detailed Instructions](https://docs.google.com/document/d/1Zf7JwQmZ9hGUo1an56qp8YnkaDlRMAUQp9nCuXUNuNs/edit?usp=sharing)**  
  Step-by-step guide for setting up inputs, running analyses, and interpreting results.

- **[Function Descriptions](https://docs.google.com/document/d/1wkXUXMdfm-RQG8Q-laYBeXXpt0ccEDsuY5Q_GiaoWXw/edit?usp=sharing)**  
  Detailed explanations of each function and its role in the ensemble workflow.

---

## Repository Link

The full set of GEE scripts is available here:  
**[Open in Google Earth Engine](https://code.earthengine.google.com/?accept_repo=users/msime/forestChangeEnsemble)**

---

## Workflow Overview

The workflow is divided into the following main components:

1. **Prepare Inputs & Configuration File**  
   Collect and generate desired forest change products and configure parameters for running the ensemble workflow.

2. **Generate Reference Data**  
   Build interpreter reference datasets that allow the validation of many change products at once.

3. **Naive Average Map**  
   Combine selected disturbance products into an average probability of forest loss without any weighting.

4. **Random Forest Ensemble**  
   Train and apply a random forest model using change products as predictors to generate forest loss maps that reflect the interpreter probabilities.

5. **Optional Uncertainty Adaptations**  
   Optional adjustments to account for various sources of uncertainty in the disturbance detection process such as interpreter disagreement.

---

## Getting Started

Running these scripts requires you to have a GEE account already made! If you do not have this, follow the instructions below: 
**[GEE Account Creation](https://developers.google.com/earth-engine/guides/access)**

1. Open the linked GEE repository in your Google Earth Engine account.  
2. Follow instructions in the **Detailed Instructions** google document.  
3. Follow the workflow steps in sequence, starting with input preparation and configuration file setup. If you are planning to use the already existing training data for Cambodia in 2022, some steps can be skipped. 

---

## Next Steps

Once you have completed the workflow:

- Use the probabilistic loss maps for monitoring, reporting, or further analysis.  
- Integrate results with additional spatial datasets for context-specific applications.

---

## Notes:

- Feel free to submit issues or pull requests for improvements to documentation.
