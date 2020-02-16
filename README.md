# Gunshot-Detection-in-Audio
**Note:** Code for RNN model & audio synthesis is not opensourced yet.
Audio classification using deep learning implemented using TensorFlow 2.0 to detect Gunshots. 97.5% test set accuracy and 
99% training set accuracy was achieved on Binary-Urban8K. This work was done during my summer internship at TUKL-NUST lab.
Due to proper preprocessing & feature extraction, a simple CNN model is used to achieve promising results. 

## Project Includes
 - Project Notebook
     - Binary_Urban8K dataset visualization
     - Preprocessing and feature extraction using Librosa library
     - Pipelines for Preprocessing
     - Training using Keras, TensorFlow 2.0
     - Predictions on:
       - Test files
       - Multiple selected files
       - Real-time sound input
- MISC Scripts Directory: it includes all the notebooks used to modify Urban8K dataset.
- Backups Directory: it contains *model weights* and *stored dataframe having features extracted from audio.*

## Dataset Details
**Note:** scripts used to modify the data are also provided in the MISC Scripts directory.
 - UrbanSound8K was extended by adding 2400 gunshot files to it from AudioSet & MIVIA audio events data set. 
     
    - "UrbanSound8K.csv" was modified accordingly.

- 74 more gunshots were added which were downloaded from:
http://soundbible.com/tags-gun.html

    - "UrbanSound8K-modified.csv" was created for latest version of dataset.
    - "US8K-Binary" refers to new dataset

- Moreover, UrbanSound8K was changed for binary classification with new classes: 
    - no_gun_shot (8358 files, which is 3 times when compared with other class.)
    - gun_shot (2848)
    - Total files are 11206.
    
- Finally, folds in dataset were increased from 10 to 40 to make it work on computers with less RAM memory.
   
## Other Details
- Currently, dataset is missing from the repository but a download link will be added soon.
- Dataframes having extracted features of dataset files are saved as `dataframes_backup.h5` in `Backups` sub-directory.
- Model with best results is also saved in `Backups` folder named as `best_weights_modified.hdf5`.

