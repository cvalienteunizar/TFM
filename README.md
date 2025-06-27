# TFM - Detection and tracking of sheep flocks from aerial images for learning the dynamic behavioral model

Author: Cintia Valiente Bermejo
Master in Robotics, Graphics and Computer Vision - ESCUELA DE INGENIERÍA Y ARQUITECTURA of Zaragoza

It contains the video results of the different experiments performed with the different predictive models of movement, Long Short-Term Memory (LSTM) networks and Parameter Identification. The videos represent the comparison between the predicted positions and the ground truth positions.

The directory is organized as follows:
- Pos-LSTM. Corresponds to the results of experiments with the Absolute Position LSTM model and synthetic data.
- Vel-LSTM. Corresponds to the experiments with the Relative Velocity LSTM model and synthetic data.
- Parameter Identification. Corresponds to the experiments with the Parameter Identification model and synthetic data.
- Video prediciton. Corresponds to the results of the experiments with the Pos-LSTM and Parameter Identification models with data extracted from a real video.

In addition, within each directory is specified the scenario to which the experiments with different numbers of sheep belong. In the case of the experiments with synthetic data there are four scenarios:
1. No-Dog: a system where only sheep interact with each other.
2. Always-Dog: the dog continually interacts with the flock by moving through or near it. 
3. Distant-Dog: the dog consistently remains far from the sheep and does not influence their behavior.
4. Rand-Dog: the dog alternates between approaching the flock and moving away.

In addition, the two inference strategies for prediction have been marked in each file as follows:
- Teacher Forcing --> TF
- Autoregressive --> AR
