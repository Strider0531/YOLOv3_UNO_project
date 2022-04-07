This YOLOv3_UNO_project is the modified TensorFlow-2.x-YOLOv3 project.

Link on TensorFlow-2.x-YOLOv3:
GitHub : https://github.com/pythonlessons/TensorFlow-2.x-YOLOv3
================================================================

YOLOv3_UNO_project configured for UNO cards recognition. Example image of YOLOv3 algorithm - img_after_yolo.jpg image whitch is on static/images directory.

Using of UNO cards recognition project:

- Recognition from image:

Open Flask_Api_YOLO_ngrok.ipynb notebook, put ngrok token on the second cell and run all cells. Use webpage for uploading UNO card image (in jpg, JPEG format). Click on "predict image" button, after that API must demonstrate resulted image with bounding boxes. 

- Recognition from webcam (using of GPU highly recommended):

Open detection_custom_notebook.ipynb. Change os.environ['CUDA_VISIBLE_DEVICES'] = '0' by os.environ['CUDA_VISIBLE_DEVICES'] = '-1' in case if you want to use CPU instead of GPU. Run cell and after that, python must create window with webcam video. Demonstrate some UNO card. Bounding boxes must be created and viewed on cards in realtime.

Training of custom YOLOv3 model in Colab:

Use YOLOv3_colab_training.ipynb. Follow tips that are mentioned in tutorial bellow.

This project is descriptioned by very informative tutorials. Link on Colab YOLOv3 training tutorial: 

https://www.youtube.com/watch?v=kIs9aftuIvE&list=PLbMO9c_jUD473OgrKYYMLRMEz-XZjG--n&index=5&ab_channel=PythonLessons

  


