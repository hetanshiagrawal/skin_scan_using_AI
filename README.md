# SkinScanAI - Identify the affected skin region and predict the type of skin cancer based on the lesion.

The described project aims to address the challenges faced by dermatologists in locating cancerous and malignant skin lesions accurately and predicting skin lesion type. The proposed solution involves a neural architecture based on convolutional neural networks (CNNs) to extract essential features from skin lesions and generate precise masks that define the lesion area. The key components and outcomes of the project include:

**1) Datasets:**
* https://www.kaggle.com/datasets/surajghuwalewala/ham1000-segmentation-and-classification
* The study uses a dataset comprising 10,000 images and masks for seven types of skin lesions:
     1.) Actinic keratoses and intraepithelial carcinoma(AKIEC):  Rough, scaly patches on the skin caused by sun damage is an early form of skin 
                                                                   cancer that is confined to the outer layer of the skin. \
     2.) Basal cell carcinoma(BCC): Most common type of skin cancer, usually appearing as a pearly or waxy bump. \
     3.) Benign keratosis-like lesions(BKL): Harmless and non-cancerous growths resembling keratosis, such as seborrheic keratosis.\  
     4.) Dermatofibroma(DF): Non-cancerous benign skin growth that often appears on the lower legs.\
     5.) **Melanoma(MEL)**: Most dangerous type of skin cancer that develops from pigment-containing cells called melanocytes. \
     6.) Melanocytic nevi(NV): Non-cancerous benign, pigmented growths on the skin commonly known as moles. \
     7.) Vascular lesions(VASC): Most are benign, meaning they are not cancerous. However, certain rare types, like angiosarcoma, can be malignant.\
* Data augmentation techniques, such as horizontal and vertical image rotation, are employed to increase the dataset size, resulting in 30,000 images 
  and 30,000 masks.

**2) Training and Testing:**
* The dataset is split into training, validation, and testing sets.
* During training, 3,500 images and masks are used for verification and adjusting neural network parameters.
* After training, the neural network is tested on 1,000 images to evaluate its performance.

**3) Neural Architecture:**
* The project utilizes a convolutional neural network, a type of deep learning model designed for image analysis tasks.
* The neural network is trained to extract features from skin lesions, which are crucial for accurately determining the location and spread of cancerous tumors and predicting type of skin lesions.

**4) Mask Generation:**
* The extracted features are used to generate masks that precisely define the area of the skin lesion. These masks aid in identifying the location 
  and boundaries of cancerous tumors.
  
**5) Lesion Type Prediction:**
* The extracted features are also used to predict lesion label using proper loss functions



**Sample Images**
![sample_images](https://github.com/PriyanshiAgrawal1345/SkinScanAI/assets/128245760/44c4ffac-7f6c-40f0-ad8d-c3169cbba2ab)

**Prediction of TestLabels**
![output_PredictedLabels](https://github.com/PriyanshiAgrawal1345/SkinScanAI/assets/128245760/2b681a82-5e51-47d2-a3f4-d3f869969922)
Accuracy: 69.5%

**Prediction of Masks of testImages**
![predictedTestMasks](https://github.com/PriyanshiAgrawal1345/SkinScanAI/assets/128245760/4b0cce12-088f-465e-b88b-fb6d30b95450)


**PerformanceEvaluationValidationMasks**
![PerformanceEvaluationValidationMasks](https://github.com/PriyanshiAgrawal1345/SkinScanAI/assets/128245760/26f87069-b670-4e27-98e8-139249546230)
