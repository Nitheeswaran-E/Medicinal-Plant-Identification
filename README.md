# Medicinal-Plant-Identification

This project revolves around the utilization of Medicinal plants for medicinal purposes. With numerous plants present in our surroundings, often with unknown uses and specifications, a Machine Learning (image recognition) model has been developed. This model can effectively detect and identify plants based on leaf images, subsequently providing relevant information about the identified plant. The model underwent training using 280 images across 6000 epochs . The accuracy achieved for image predictions stands at approximately 9.45334.

All necessary resources, including codes for data categorization, prediction, plant dataset, and required files, can be found on the project's GitHub repository. Additionally, the repository includes an image annotation software . Certain adjustments are essential before initiating the training process. When uploading the classes.txt file, it should be subsequently saved with the extension (.names) after reopening it on your device, specifically named as classes.names. This file is pivotal for labeling images by classes during model training. Once created, the file should be uploaded to the images folder.

Within the training_model code, there is a segment dedicated to generating train.txt, test.txt, and labelled_data.data files. It's imperative to verify the presence of these files in the image folder. Both train.txt and test.txt should include paths to the training images. For reference, I've provided my own files in the "files for training" folder.

To ensure data safety, establish a backup folder in the same drive location as the image and darknet folders. After executing the code in training_model, double-check the modifications in the make file.

Open this file using a text editor and implement specific modifications. Uncomment relevant lines for testing and training, adjust numbers for batch and subdivisions based on your dataset division. Determine the "max_batches" value for setting the number of epochs (consider 3000 if using Collab due to runtime disconnection). Introduce numbers within the "steps" parameter between the "max_batches" numbers, maintaining a difference of approximately 20 to 30.


Upon completion, the model will automatically save within the backup folder alongside the epoch graph, using the .weights extension. If the darknet function encounters issues in Collab, a code named "cmd" can provide access. The model can be downloaded from the provided Google Drive link: Model Download Link.
