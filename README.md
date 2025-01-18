**Creating a computer vision model for classifying ocular artifacts in EEG data**

EEG data requires cleaning and preprocessing before the electrical signals can be analysed by researchers. Muscle movements, blinks, and external activity cause artifacts which obscure important signals. Automatic removal of these artifacts is handled by algorithms, but they are currently not reliable enough to be used in isolation in most cases - trained researchers are required to visually inspect the data before deciding if an artifact is present.  
  
By training a computer vision model on topoplots of both artifacts (in our case, blinks) and negative data we can teach it to classify ocular artifacts. We can then use the model in our preprocessing pipeline to remove them automatically with human accuracy - thousands of times faster, and without the expertise.

Here is a **general overview** of the project:
1. Downloading public datasets, and processing the data for training.
2. Training the model on the processed data.
3. Testing and evaluating the model.
