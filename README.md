# UESim_feedback

## Setting up the sim

### Start the Estimator(Keypoint network)
- Start term
- Navigate to CNN folder: `cd Documents/projects/NN_attitude`
- Start the conda environment: `conda activate nn_attitude`
- Run the estimator: `python3 predict_server.py`
  - This scirpt waits for an image to appear in folder `Documents/projects/ue_images` and saves the result in a csv file in `cnn_estimate.csv`   
  
