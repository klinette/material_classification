# material_classification
Multimodal Material Classification and Sound Prediction from Visual Scenes

Final project for MIT's Advances in Computer Vision class (6.8300), Spring 2023

## Description
We investigated the use of visually indicated sounds by adding sound to silent video frames of drumsticks hitting different materials from the Greatest Hits dataset. Our first goal was to determine if combining both image and sound information improved our ability to predict the material being hit compared to using a single modality. To achieve this, we explored a range of neural network architectures and parameters. Our second objective was to create a model that takes in video frames of hits and returns a one-second audio clip corresponding to the hit using a state-of-the-art convolutional neural network. To prepare the data, we took singular frames at the exact moment of contact between the drumstick and the object and cropped the one-second audio file centered around the hit. Our findings indicate that combining both image and sound information leads to more accurate predictions of the material in new images and sounds. We were also able to create 1-second audio clips that are louder at the time of the hit. However, our audio clips are noisy and do not change depending on the material being hit, which we attribute to limited computational power and the temporal dependencies inherent in spectrograms that our model does not consider.
