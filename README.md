# data-labelling
!pip install roboflow

from roboflow import Roboflow
rf = Roboflow(api_key="X9JTcM843YXy92aZdieP")
project = rf.workspace("anotate-wvfjm").project("brain-teumer-detection-almz3")
version = project.version(3)
dataset = version.download("yolov11")
                
