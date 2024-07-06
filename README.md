# Driver-Drowsiness-Facial-Image-Analysis-


### Objective
To develop and analyze models for detecting driver drowsiness using images, aiming to improve road safety by identifying when drivers close their eyes for extended periods.

### Business Objective
To leverage technology in preventing accidents caused by driver drowsiness, thereby reducing insurance claims, enhancing policy pricing, and enabling dynamic policy customization for insurance companies.

### Dataset Overview
The datasets used include:
- **MRL Eye Dataset**: Contains close-up images of eyes with information on gender, glasses reflection, and lighting conditions.
- **Closed Eyes in the Wild**: Includes facial images with annotations for eyes, nose, mouth, and other facial features.
- **Driver Face Dataset**: Comprises image sequences of subjects driving, with annotations for facial key points and gaze direction.

### Analysis Approach
1. **Data Collection**:
   - Gathered datasets from sources like MRL Eye Dataset, Closed Eyes in the Wild, and Driver Face Dataset.
   - Images included both open and closed eye states under various conditions.

2. **Feature Extraction**:
   - Used Histogram of Oriented Gradients (HOG) to capture eye structure.
   - Applied SVM classifier to distinguish between open and closed eyes.

3. **Model Training**:
   - Utilized Convolutional Neural Network (CNN) in TensorFlow for binary image classification.
   - Implemented EfficientNet architecture for optimal balance between accuracy and computational efficiency.
   - Trained models using batch normalization and dropout techniques to reduce overfitting.

4. **Testing and Evaluation**:
   - Evaluated models on different datasets to assess performance.
   - Conducted external dataset testing to ensure robustness and generalizability.

### Insights
1. **Model Performance**:
   - EfficientNet demonstrated superior balance between accuracy and computational efficiency.
   - Models trained on MRL dataset achieved the highest accuracy (94.45%) compared to other datasets.
   - Overfitting was identified as a challenge, impacting out-of-sample performance.


2. **Business Impact**:
   - Real-time application for accident prevention involves installing a video camera in the car, feeding live footage through a trained CNN, and triggering an alarm if the driver closes their eyes for an extended period.
   - Insurance companies can benefit from reduced claims costs, automated monitoring, and enhanced policy pricing through risk profiling.

### Recommendations
1. **Model Improvement**:
   - Test other model architectures and classification methods to enhance performance.
   - Create higher thresholds for closed eyes classification in real-time applications to avoid over-penalizing insured drivers.
   - Choose and tune models based on the specific camera setup and images that will be classified.

2. **Dataset Expansion**:
   - Acquire more labeled datasets with images of people with their eyes open and closed for better out-of-sample performance testing.
   - Factor in environmental conditions like rural roads, highways, and time of day when capturing images.

3. **Additional Features**:
   - Explore the impact of audio selection on driver drowsiness by designing experiments with different genres of music and evaluating classifiers on eye status.

4. **Business Applications**:
   - Implement the drowsiness detection system in vehicles to alert drivers and prevent accidents.
   - Utilize insights for dynamic policy customization and risk profiling in insurance to offer tailored policies.

These insights and recommendations will help in developing a robust driver drowsiness detection system, ultimately enhancing road safety and providing significant benefits to insurance companies.
