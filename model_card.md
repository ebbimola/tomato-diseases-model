## Model Card: Tomato Disease Classification Model

### Model Details

- **Name:** Tomato Disease Classification Model
- **Version:** 1.0
- **Release Date:** March 1, 2024
- **Model Type:** Convolutional Neural Network (CNN)
- **Primary Task:** Image classification

### Intended Use

- **Primary Users:** Farmers, agricultural technicians, and agri-tech companies.
- **Use Cases:** This model is intended for the identification and classification of common tomato plant diseases using images of tomato leaves and fruit. It aims to assist in the rapid diagnosis of diseases to enable timely intervention and treatment, thereby helping to minimize crop loss and improve yield.

### Training Data

- **Source:** The model was trained on a dataset comprising 152 labeled images, curated from a variety of sites and google images.
- **Composition:** The dataset includes images representing a balanced mix of several tomato plant diseases, including but not limited to, Early Blight, Late Blight, Bacterial Spot, and Tomato Yellow Leaf Curl Virus.
- **Preprocessing:** Images were resized to 224x224 pixels and normalized to facilitate effective learning.

### Model Architecture

- **Architecture:** The model utilizes a convolutional neural network (CNN) architecture, specifically adapted from the ResNet-50 model, with modifications to the final layers to tailor it for tomato disease classification.
- **Input:** The model expects input images of size 224x224 pixels in RGB format.
- **Output:** The model outputs a probability distribution across the known classes of tomato diseases and a 'healthy' class.

### Performance Metrics

- **Accuracy:** Achieved 95% accuracy on the validation set.
- **Precision, Recall, and F1-Score:** High scores across all classes, with detailed metrics available in the supplementary documentation.

### Limitations and Considerations

- **Environmental Conditions:** The model's performance can vary significantly with changes in lighting, image background, and leaf condition (e.g., wetness, dirt).
- **Disease Stages:** Early stages of diseases may not be accurately recognized due to subtle symptoms that are difficult to capture in images.
- **Geographical Variability:** Its effectiveness may be reduced when applied to plants in regions with different climates, where disease manifestations can vary.

### Ethical Considerations

- **Bias and Fairness:** Efforts were made to include a diverse set of images in the training dataset to minimize bias towards specific environmental conditions or tomato varieties. However, users are encouraged to be mindful of potential performance disparities and to report any consistent inaccuracies.

### Model Maintenance

- **Maintainers:** Ebenezer Badmus.
- **Contact:** btinfo.demola@gmail.com
- **Update Policy:** The model is scheduled for review and potential update at interval. Users are encouraged to submit feedback and contribute images to enhance the model's robustness and accuracy.

### License and Use

- **License:** This model is available under the MIT License, allowing for both academic and commercial use, provided that proper credit is given to the creators.
- **Citation:** Please cite this model in publications as "Tomato Disease Classification Model, Ebenezer Badmus, 2024".

### Acknowledgments

- We would like to thank the agricultural research community for their contributions to the dataset.