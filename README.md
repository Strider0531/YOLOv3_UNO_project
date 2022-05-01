This YOLOv3_UNO_project is the modified TensorFlow-2.x-YOLOv3 project.

================================================================

Project developed in Python 3.7

YOLOv3_UNO_project configured for UNO cards detection.

Using of UNO cards recognition project:

- Image detection:

Open Flask_Api_YOLO_ngrok.ipynb notebook, put ngrok token on the second cell and run all cells. Use webpage for uploading UNO card image (in jpg, JPEG format). Click on "predict image" button, after that API must return resulted image with bounding boxes. 

![alt text](https://github.com/Strider0531/YOLOv3_UNO_project/blob/master/static/images/img_after_yolo.jpg?raw=true)

- Detection with webcam (using of GPU highly recommended):

Open detection_custom_notebook.ipynb. Change os.environ['CUDA_VISIBLE_DEVICES'] = '0' by os.environ['CUDA_VISIBLE_DEVICES'] = '-1' in case if you want to use CPU instead of GPU. Run cell and after that, python must create window with webcam video. Demonstrate some UNO card. Bounding boxes must be created and viewed on cards in realtime.

![alt text](https://github.com/Strider0531/YOLOv3_UNO_project/blob/master/IMAGES/web_example.jpg?raw=true)

- Training of custom YOLOv3 model in Colab:

First of all you should prepare custom dataset. Open XML_to_YOLOv3.py and set data_dir to your dataset folder with images and their XML's files. Also set Dataset_train, Dataset_test and Dataset_names_path for .txt files saving.

Secondly, you should open yolov3/configs.py and set next configs:
  1. TRAIN_CLASSES (.txt file saved by Dataset_names_path)
  2. TRAIN_ANNOT_PATH (.txt file saved by Dataset_train)
  3. TRAIN_MODEL_NAME (configurate model name)
  4. TEST_ANNOT_PATH (.txt file saved by Dataset_test)
 
 Also you can change other configs. For more information follow tips that are mentioned in project tutorial bellow.

https://www.youtube.com/watch?v=kIs9aftuIvE&list=PLbMO9c_jUD473OgrKYYMLRMEz-XZjG--n&index=5&ab_channel=PythonLessons

=======================================================================

Link on TensorFlow-2.x-YOLOv3:
GitHub : https://github.com/pythonlessons/TensorFlow-2.x-YOLOv3  
