# Segway

Simulate a Segway with a person driving at low speed and passing obstacles

## Description
We simulated the Segway with a pid controller, and realized that the manned Segway can maintain balance in the simulated park and pass through multiple obstacles. This is because we use the PID controller to control the error of the angle, so that the Segway's handrail and the ground remain close to 90 degrees. Because the reference is the ground (the floor inside MUJOCO), the Segway can run upright on any slope at 90 degrees relative to the ground. The steering of Segway is achieved by increasing the torque of one wheel on the basis of PID control to make the wheel turn faster. This model was made with MUJOCO.

In addition, we have a version that uses QLearning to realize the manned Segway to maintain balance and drive forward.

## Getting started

To make it easy for you to get starte, here's a list of recommended next steps.

### Download files

Download Segway.zip in elearning


### Unzip Segway.zip
Segway.zip contains two folders, SegwayPID and SegwayQLearning.


Segway-v5.ipynb is included in folder SegwayPID. A modelPark.xml. a renderer.py. There are also several .stl files stone3Rock_15_Low.stl, stone1Rock_18_low.stl, seesaw_pole2.stl, seesaw_pole1.stl, ramp.stl, planttree.stl, plant_stand_middle.stl, plant_stand.stl, model_upper_torso.stl, model_short.stl, model_shirt_010.stl, model_right_shoe.stl, model_right_pupil.stl, model_right_palm.stl, model_right_forearm.stl, model_right_eye.stl, model_right_arm.stl, Model_new_trousers.stl, Model_left_shoe.stl, model_left_pupil.stl, model_left_palm.stl, model_left_forearm.stl, model_left_eye.stl, model_left_arm.stl, model_head.stl, model_hair.stl, floor.stl, bridge.stl  and several .obj files Tire.obj, Dog.obj, CoconutHalfm.obj, CoconutHalf.obj.

Segway-v0.ipynb is included in folder SegwayQLearning. A modelv2.xml. a renderer.py. There are also several .stl files model_upper_torso.stl, model_short.stl, model_shirt_010.stl, model_right_shoe.stl, model_right_pupil.stl, model_right_palm.stl, model_right_forearm.stl, model_right_eye.stl, model_right_arm.stl, Model_new_trousers.stl, Model_left_shoe.stl, model_left_pupil.stl, model_left_palm.stl, model_left_forearm.stl, model_left_eye.stl, model_left_arm.stl, model_head.stl, model_hair.stl and several .obj files Tire.obj, CoconutHalfm.obj, CoconutHalf.obj.


### Dependencies

Jupyter notebooks via the "Physx HCI 2" kernel

MUJOCO

Blender is also required if the model's .stl files need to be changed.


### Executing program
In order to view and edit models in modelPark.xml, the following steps should be performed:

1.  - [ ] [Download the mujoco simulate]([https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file](https://github.com/deepmind/mujoco/releases) 
2.   make sure that .obj, .stl, .xml renderer.py files are in a same folder
3.  drag the .xml file to the centre of mujoco simulate


Jupyter notebook:
1. Upload all files under the .zip file to JupterLab.
2. Open the .ipynb file.
3. Set Kernel to Physx HCI 2 to ensure that all dependent libraries are in the environment.
4. Click: Kernel - Restart Kernel and Run all Cells.

Remarks, wait for a while to see the video of Segway-v5.ipynb running. For Segway-v0.ipynb, it needs to run for a long time to gradually generate multiple videos to show the training results. Your patience is required here.

## Authors

Gaogianq Liu, 
Lian Thung Lee , 
Louise Schaub, 
Rawen jendoubi, 
Robin Schmeußer,
Yucong Zhang

