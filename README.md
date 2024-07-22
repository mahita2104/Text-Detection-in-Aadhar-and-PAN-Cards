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

The system uses a dataset from Kaggle, with annotations performed using VoTT (Visual Object Tagging Tool) to ensure accurate detection and classification of these text fields.

## Results

The YOLOv3 model demonstrates effective detection of text fields, achieving the following performance metrics:
- **Accuracy:** 93% on the validation set
- **Precision:** 91% for text field detection
- **Recall:** 94% for identifying text fields

Sample detection results include accurate identification and localization of text fields such as names, IDs, and other critical information in Aadhaar and PAN cards. For visual examples, see the sample images in the `results/` directory.

## Future Scope

- **Enhanced Accuracy:** Further refinement of the model to improve precision and recall.
- **Support for More Documents:** Extending detection capabilities to include additional types of identification documents.
- **OCR Integration:** Implementing Optical Character Recognition (OCR) to extract and process detected text fields for automated data entry and analysis.
- **Fake ID Detection:** Developing methods to use the detection system for identifying and verifying the authenticity of ID cards, potentially flagging counterfeit or forged documents.
- **Real-Time Processing:** Development of real-time detection capabilities for practical applications.
- **Integration:** Potential integration into document verification and management systems.

## Acknowledgements

- **YOLOv3:** Developed by Joseph Redmon and collaborators, available at [Darknet GitHub Repository](https://github.com/pjreddie/darknet).
- **VoTT:** Visual Object Tagging Tool by Microsoft, available at [VoTT GitHub Repository](https://github.com/microsoft/VoTT).
- **Dataset:** [Personal Identification Image Dataset for India](https://www.kaggle.com/datasets/mehaksingal/personal-identification-image-dataset-for-india) by Mehak Singal on Kaggle.
