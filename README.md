# Towards Transparency in Black-Box Models: A Brief Review of Methods in Explainability for AI Systems

## Author
**Saleh Alkhalifa**  
Northeastern University

---

## Overview
This project focuses on enhancing transparency and interpretability in AI systems operating in sensitive and regulated environments such as life sciences, biopharmaceuticals, and healthcare. By leveraging various datasets and machine learning models, it evaluates different explainability methods like SHAP, LIME, Integrated Gradients, and Token-Level Attributions to provide insights into model decision-making. The ultimate goal is to bridge the gap between the performance of complex models and the interpretability required in high-stakes scenarios.

---

## Objectives
- **Address the Black-Box Problem**: Investigate the decision-making processes of AI models to ensure transparency and trustworthiness.
- **Implement Explainability Techniques**: Apply methods such as SHAP, LIME, Integrated Gradients, and Attribution to uncover hidden patterns in data and models.
- **Explore Diverse AI Models**: Cover regression, classification, and generative AI models, as well as deep learning architectures.
- **Evaluate in Regulated Environments**: Provide insights relevant to compliance, ethical considerations, and operational transparency in industries like pharmaceuticals and healthcare.

---

## Quick Links
- **[Article PDF](https://github.com/alkhalifas/Towards-Transparency-in-Black-Box-Models/blob/main/deliverables/CS6140%20Final%20Report%20Group%201%20Report.pdf)**: Download the detailed research article in PDF format.
- **[Article Summary on Medium.com](https://medium.com/ai-mind-labs/understanding-explainable-ai-xai-and-its-importance-in-modern-ai-systems-43ffc816991d)**: Read the summarized article on Medium.
- **[Video Presentation](https://youtu.be/IYmoKeNvDT0)**: Watch the video presentation of the project.
- **[PowerPoint Slide Deck](https://github.com/alkhalifas/Towards-Transparency-in-Black-Box-Models/blob/main/deliverables/CS%206140%20Project.pptx)**: View the PowerPoint slide deck.

---

## Datasets Used
1. **California Housing Dataset** (Regression): Predict median house values with structured input features.
2. **Breast Cancer Dataset** (Classification): Binary classification of malignant and benign tumors.
3. **AG News Dataset** (Generative AI): Text classification to evaluate token-level attributions.
4. **Sentiment Analysis Data** (Closed Source Generative AI): Sentiment classification with proprietary GPT-4o model.
5. **MNIST Dataset** (Deep Learning): Handwritten digit classification for pixel-level attributions.

---

## Models Implemented
### 1. Ridge Regression (Discriminative - Regression)
- Dataset: California Housing
- Explainability: SHAP and LIME
- Key Insights:
  - SHAP provided global feature importance, revealing the influence of features like median income and average rooms.
  - LIME delivered instance-specific explanations for individual predictions.

### 2. Random Forest Classifier (Discriminative - Classification)
- Dataset: Breast Cancer
- Explainability: SHAP and LIME
- Key Insights:
  - Random Forests excelled in capturing non-linear relationships.
  - SHAP identified critical features like mean radius and texture, enhancing interpretability for medical diagnosis.

### 3. DistilBERT (Generative AI - Open Source)
- Dataset: AG News
- Explainability: Integrated Gradients
- Key Insights:
  - Token-level attributions highlighted the importance of key words in text classification tasks.
  - Demonstrated strong alignment between model predictions and human linguistic intuition.

### 4. GPT-4o (Generative AI - Closed Source)
- Dataset: Sentiment Analysis
- Explainability: Token-Level Attributions via Masking
- Key Insights:
  - Used prompt engineering to infer model behavior despite proprietary restrictions.
  - Highlighted the influence of specific emotional descriptors on sentiment predictions.

### 5. Neural Network (Deep Learning)
- Dataset: MNIST
- Explainability: Integrated Gradients
- Key Insights:
  - Pixel-level attributions confirmed the model’s focus on key features of handwritten digits.
  - Validated the network’s reasoning against human expectations.

---

## Explainability Techniques
### 1. **SHAP**:
- Assigns feature importance using Shapley values.
- Ideal for global and local interpretability in structured data.

### 2. **LIME**:
- Provides instance-specific explanations.
- Effective for understanding individual predictions.

### 3. **Integrated Gradients**:
- Attributes predictions to input features by integrating gradients.
- Best suited for deep learning and generative models.

### 4. **Token-Level Attributions**:
- Evaluates the impact of individual words or tokens on model predictions.
- Used for open and closed-source generative AI.

---

## Results
- Ridge Regression with SHAP and LIME revealed interpretable patterns in housing data.
- Random Forest and SHAP provided insights into key diagnostic features in breast cancer classification.
- Integrated Gradients offered detailed visualizations for both textual and image-based models.
- GPT-4o’s explainability was partially achieved through prompt engineering and masking techniques.

---

## Visualizations
- Feature Importance (SHAP): Highlighted global and local feature impacts.
- Token Attributions (Integrated Gradients): Showed positive and negative contributions for text classification.
- Pixel Attributions (MNIST): Demonstrated which strokes contributed most to digit recognition.

---

## Conclusion
This project highlights the importance of explainability in AI, particularly in high-stakes environments. By combining various datasets, models, and explainability methods, it offers a comprehensive framework for understanding model decisions, fostering trust and compliance in AI systems.

---

## Future Work
- Develop hybrid explainability frameworks combining global and local methods.
- Investigate fairness and bias through interpretability techniques.
- Extend analysis to more complex datasets and generative tasks.

---

## References
1. Lundberg, S. M. (2017). *A Unified Approach to Interpreting Model Predictions*.
2. Ribeiro, M. T., Singh, S. (2016). *Why Should I Trust You? Explaining the Predictions of Any Classifier*.
3. Sundararajan, M., Taly, A. (2017). *Axiomatic Attribution for Deep Networks*.
4. Vig, J. (2019). *A Multiscale Visualization of Attention in the Transformer Model*.
5. Selvaraju, R. R., et al. (2017). *Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization*.

---

## How to Use
1. Clone the repository:
   ```bash
   git clone git@github.com:alkhalifas/Towards-Transparency-in-Black-Box-Models.git
