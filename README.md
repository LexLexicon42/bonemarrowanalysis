# Pediatric Bone Marrow Transplant Survival Classification

## Introduction
Unmanipulated allogeneic hematopoietic stem cell transplantation is a commonly used and effective treatment for children with various hematologic diseases, both malignant and nonmalignant. This treatment functions by transplanting healthy CD34+ stem cells from an unrelated donor to the afflicted child. It has been proven in Kałwak et al.’s 2010 study that higher doses of CD34+ stem cells are associated with a higher chance of survival for the recipient and a lower chance of relapse, without increased risks of severe side effects. Prior research indicates that certain factors are influential in predicting a child’s chance of survival following the transplant, including the age of the donor and recipient, the recipient’s body mass, and the dosage of CD34+ stem cells administered to the patient.

Using the bone marrow transplant dataset available to us, can we predict whether a future pediatric patient with a hematologic disease who receives a bone marrow transplant is likely to survive or not based on the predictors of donor age, recipient age, CD34+ cell dose, and body mass?

The dataset describes cases of pediatric patients with malignant hematologic diseases such as acute lymphoblastic leukemia, acute myelogenous leukemia, chronic myelogenous leukemia, and myelodysplastic syndrome as well as nonmalignant hematologic diseases such as severe aplastic anemia, Fanconi anemia, and X-linked adrenoleukodystrophy. All of the patients in the dataset had unaltered allogeneic unrelated donor hematopoietic stem cell transplants. These are the five different predictors used to answer our question:

- Donor_Age - Age of the donor when hematopoietic stem cells were removed
- Recipient_Age - Age of the recipient when the hematopoietic stem cells were transplanted
- CD34_Dose - CD34+ cell dose per kg of recipient body weight (10^6 cells/kg)
- Body_Mass - Body mass of the recipient at the time of transplantation
- Survival_Status - The survival status of the recipient after the transplant (0 = deceased, 1 = survived)

## Methods and Results
### Group Collaboration
This project was conducted collaboratively with a group.

### Software Requirements
- tidyverse
- tidymodels
- dbplyr
- GGally
- ggplot2

### Data Preparation
The dataset was read into R and cleaned to ensure it was in a tidy format suitable for analysis.

### Exploratory Data Analysis
Exploratory data analysis was conducted to understand the distribution of variables and relationships within the dataset.

### Preprocessing and Model Building
- Data preprocessing steps, including scaling, were performed.
- A k-nearest neighbors classification model was trained and tuned using cross-validation.
- The model's accuracy was evaluated on both training and testing datasets.

### Results
- The accuracy of the model derived from cross-validation was observed to be 64.5%.
- When tested on the testing set, the model's accuracy dropped to 55.3%.
- A confusion matrix was generated to analyze the model's performance.

## Discussion
The results suggest that the predictor variables may not be sufficient to accurately predict a patient's survival status following a bone marrow transplant. Further research is needed to identify additional factors that may influence survival outcomes.

## Future Questions
- How can the chances of survival of future patients be improved?
- How can the donor’s compatibility with the recipient be optimized?
- What are the main factors impacting a patient’s survival status?

## References
- Kałwak, Krzysztof, et al. “Higher CD34+ and CD3+ Cell Doses in the Graft Promote Long-Term Survival, and Have No Impact on the Incidence of Severe Acute or Chronic Graft-versus-Host Disease after In Vivo T Cell-Depleted Unrelated Donor Hematopoietic Stem Cell Transplantation in Children.”
- Sikora, Marek, and Lukasz Wrobel. “Bone Marrow Transplant: Children.” UCI Machine Learning Repository.
- Sikora, Marek, et al. “Application of Rule Induction to Discover Survival Factors of Patients after Bone Marrow Transplantation.”

---
*This project was conducted as part of a collaborative effort with group members.*
