# Gunshot-Detection-using-Audio
 Deep learning model is implemented using TensorFlow 2.0 to detect Gunshots. 97.5% testing set accuracy and 99% training set accuracy was achieved using TensorFlow 2.0. 

## Project Includes
- Project Notebook
 - Audio dataset visualization
 - Preprocessing and feature extraction using Librosa library
 - Training using Keras, TensorFlow 2.0
 - Prediction on:
   - Test files
   - Multiple selected files
   - Real-time sound input
- Utils Directory: it includes all the notebooks used to modify Urban8K dataset.
- Backups Directory: it contains *model weights* and *stored dataframe having features extracted from audio.*

## Dataset Details
 **Dataset Details**
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
    
- FinallY, folds in dataset were increased from 10 to 40 to make it work on computers with less RAM memory.
   
## Other Details
- Currently, dataset is missing from the repository but a download link will be added soon.
- Dataframes having extracted features of dataset files are saved as `dataframes_backup.h5` in `Backups` sub-directory.
- Model with best results is also saved in `Backups` folder named as `best_weights_modified.hdf5`.

