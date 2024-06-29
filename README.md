# UESim_feedback

## Setting up the sim

### Start the Estimator(Keypoint network)
- Start term
- Navigate to CNN folder: `cd Documents/projects/NN_attitude`
- Start the conda environment: `conda activate nn_attitude`
- Run the estimator: `python3 predict_server.py`\newline
This scirpt waits for an image to appear in folder `Documents/projects/ue_images` and saves the result in a csv file in `cnn_estimate.csv`
   
### Start Rendring Engine
- Start Unreal Engine
  - Start terminal from desktop and run the startup shell script : `./unreal.sh`
  - Alternatively from term, run : `/opt/Linux_Unreal_Engine_5.1.1/Engine/Binaries/Linux/./UnrealEditor`      
  - From `Recent Projects` tab, select `Browse` and navigate to `home/mist/Documents/UnrealProjects/RainSIm` folder. Select and open the `RainSIm.uproject` file to run the project in UE.\newline
This project contains all the assets required to run single agent or multiagent target satellite tracing problem.
- Navigate to `Content Drawer` folder from a tab on the bottom left. Run the level: `Earth_EditorMode3` by double clicking. Set window pane to Output Log to view status.

### Start the dynamics Engine (Python/Matlab)
- From term run matlab: `matlab`
- Navigate to `/home/mist/Documents/projects/Matlab-trial-codes` and open and run the script `traj_HCW_rotated_dt_adi.m`.

### Run the python UE executor
- Navigate back to UE tab
- Goto the `Tools` menu, navigate to the bottom and run Execute Python Scripts. Navigate to folder : `home/mist/Documents/UnrealProjects/RainSIm`. Run the script `matlab_mover_socket_debug.py`

Wait  
