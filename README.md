# An-Object-Classification-approach-for-Autonomous-Vehicles-using-synthetic-data
Object detection using YOLOv3 with TensorFlow 1.15.x in Carla Simulator
# Setup
1. Download Carla 0.9.9 [https://github.com/carla-simulator/carla/releases/tag/0.9.9/] and  python 3.7.5.
2. Navigate to the Carla Simulator examples path by using the cd command. Assuming the examples path is located at ..\CARLA_0.9.9\WindowsNoEditor\PythonAPI\examples
3. Clone this repo without project folder with the below section
4.Download COCO weights from this link:
https://github.com/YunYang1994/tensorflow-yolov3/releases/download/v1.0/yolov3_coco.tar.gz
5.extract this file under the below path:
..\CARLA_0.9.9\WindowsNoEditor\PythonAPI\examples\tensorflow-yolov3\checkpoint
6.cd..
python convert_weight.py
python freeze_graph.py
7.Open CarlaEU4.exe (..\CARLA_0.9.9\WindowsNoEditor)
8.python spawn_npc.py
9.python yolov3_object_detection.py
# Project Directory Structure
.CARLA_0.9.9            
├── WindowsNoEditor
│   │   ├── CarlaUE4
│   │   ├── Co-Simulation
│   │   ├── Engine
│   │   ├── HDMaps
│   │   ├── PythonAPI
│   │   │   ├── carla
│   │   │   ├── util
│   │   │   ├── examples
│   │   │   │ 	├── yolov3_object_detection.py
│   │   │   │ 	├── tensorflow_yolov3    
│   │   │   │ 	│   │  	├── carla
│   │   │   │ 	│   │	│   ├── utils.py            
