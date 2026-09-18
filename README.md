# Image-based cycling route experiment

This repository contains the code and supporting data for the paper:

**Understanding cycling route choice behaviour through street-level images and discrete choice models**  
Roosmarijn Terra, Francisco Garrido-Valenzuela, Oded Cats, and Sander van Cranenburgh.

The study investigates cyclists' preferences for cycling environments using an image-based stated route-choice experiment. Respondents chose between hypothetical cycling routes that differed in their cycling environment, represented using real-world street-level images, travel time, and number of traffic lights.

The resulting choice data are analysed using conventional discrete choice models based on interpretable GIS-derived environmental attributes and a computer vision-enriched discrete choice model (CV-DCM) that learns relevant information directly from the street-level images.

## Repository contents

This repository contains the code used for the analyses presented in the paper, together with the processed data that can be made publicly available.

The repository includes:
- processed stated-choice and cycling-environment data (excluding the street-level images);
- code for estimating the conventional discrete choice models.

## Data

The study is based on an image-based stated-choice experiment conducted in the Netherlands. The experiment contains 11,190 observed route-choice tasks from 746 respondents and uses 6,484 unique cyclist-perspective street-level images.

The processed stated-choice and cycling-environment data are provided in this repository. The original street-level images cannot be publicly redistributed due to licensing restrictions and are therefore not included. Researchers interested in analyses requiring information derived from the images are welcome to contact the authors to discuss whether access or additional derived image features can be provided.

## Models

Three discrete choice models are considered:

1. **MNL with GIS-derived cycling-environment attributes** – estimates interpretable preferences for environmental characteristics such as cycling infrastructure, greenery, pavement, and buildings.
2. **Error Component Mixed Logit (EC-MXL)** – extends the GIS-based model to account for correlation across repeated choices from the same respondent.
3. **Computer Vision-enriched Discrete Choice Model (CV-DCM)** – integrates a computer vision model directly into the utility function to learn cyclists' preferences from street-level images.

Because the original street-level images cannot be redistributed, the CV-DCM analysis cannot be fully reproduced from the publicly available repository alone.

## Citation

If you use this repository, please cite:

> Terra, R., Garrido-Valenzuela, F., Cats, O., & van Cranenburgh, S.  
> *Understanding cycling route choice behaviour through street-level images and discrete choice models.*
