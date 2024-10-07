# Text-Detection-in-Aadhar-and-PAN-Cards
## Overview

This project focuses on detecting and identifying text fields in Aadhaar and PAN cards using the YOLOv3 model, based on the Darknet architecture. The model efficiently locates and extracts specific text fields from these personal identification documents.

In PAN cards, the following fields are detected:
- Name
- Date of Birth (DOB)
- Father's Name
- PAN Number
- Signature
- Photograph

In Aadhaar cards, the detected fields include:
- Name
- Father's Name
- Date of Birth (DOB)
- Gender
- Aadhaar Number
- QR Code
- Photograph

The system uses a dataset from Kaggle [GovtID Dataset](https://www.kaggle.com/datasets/sparsh2002/govtiddataset), with annotations performed using VoTT (Visual Object Tagging Tool) to ensure accurate detection and classification of these text fields.

## Results
Take a detailed look at the model's results , the detected objects and their bounding boxes are represented below :

- Aadhar Card
<p align="center">
  <img src="https://github.com/mahita2104/Text-Detection-in-Aadhar-and-PAN-Cards/blob/main/Results/aadhar_card_test_result.png" />
</p>

- Pan Card
<p align="center">
  <img src="https://github.com/mahita2104/Text-Detection-in-Aadhar-and-PAN-Cards/blob/main/Results/pan_card_test_result.png" />
</p>

The model successfully detected and localised the objects of interest in both Aadhaar Card and PAN cards.Each detection has been annotated directly on the image, displaying the object's label and confidence score, as shown in the provided examples.

## Applications
- **Simplied ID Verfication:** This model can assist in making everyday processes like verifying Aadhaar and PAN cards quicker and easier. Whether opening a bank account, getting a new SIM card, or accessing government services, the technology can help ensure smooth and accurate identity verification.
- **Effortless Data Entry:** Imagine reducing the manual effort involved in filling out forms or databases. By automatically extracting information from ID cards, the system can help individuals and businesses save time, making tedious data entry a thing of the past.
- **Fraud Detection** In today’s world, verifying the authenticity of documents is critical. This model can play a key role in identifying fake or altered IDs, providing an extra layer of security and helping to build trust in sensitive transactions.
- **Faster, More Efficient Service:** From airports to service counters, quick and reliable processing of ID documents can enhance customer experiences. By integrating real-time document detection, we can make these interactions faster and less stressful for both staff and users.
## Future Scope

- **Enhanced Accuracy:** Further refinement of the model to improve precision and recall.
- **Support for More Documents:** Extending detection capabilities to include additional types of identification documents.
- **OCR Integration:** Implementing Optical Character Recognition (OCR) to extract and process detected text fields for automated data entry and analysis.
- **Fake ID Detection:** Developing methods to use the detection system for identifying and verifying the authenticity of ID cards, potentially flagging counterfeit or forged documents.

## Acknowledgements

- **YOLOv3:** Developed by Joseph Redmon and collaborators, available at [Darknet GitHub Repository](https://github.com/pjreddie/darknet).
- **VoTT:** Visual Object Tagging Tool by Microsoft, available at [VoTT GitHub Repository](https://github.com/microsoft/VoTT).
- **Dataset:** [Personal Identification Image Dataset for India](https://www.kaggle.com/datasets/mehaksingal/personal-identification-image-dataset-for-india) by Mehak Singal on Kaggle.
