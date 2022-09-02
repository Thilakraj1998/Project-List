<img src="https://149695847.v2.pressablecdn.com/wp-content/uploads/2020/08/object-detection-illustration.png" width=1500 height=430>

### Object Detection

Object detection refers to the capability of computer and software systems to locate objects in an image/scene and identify each object. Object detection has been widely used for face detection, vehicle detection, pedestrian counting, web images, security systems and driverless cars. There are many ways object detection can be used as well in many fields of practice. Like every other computer technology, a wide range of creative and amazing uses of object detection will definitely come from the efforts of computer programmers and software developers.

The breakthrough and rapid adoption of deep learning in 2012 brought into existence modern and highly accurate object detection algorithms and methods such as R-CNN, Fast-RCNN, Faster-RCNN, RetinaNet and fast yet highly accurate ones like SSD and YOLO. Using these methods and algorithms, based on deep learning which is also based on machine learning require lots of mathematical and deep learning frameworks understanding. 

There are millions of expert computer programmers and software developers that want to integrate and create new products that uses object detection. But this technology is kept out of their reach due to the extra and complicated path to understanding and making practical use of it.

The system should detect objects,

* Develop Python Implementation of Object Detection
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of detection module should be saved in respective formats(has per input format).


### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/Recognition.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format

### Note

In Usage, file creates a function main() accepting single input, which can either be an image or video. Through this function, other required functions to make detection should be called and return output in the appropriate format.

**Example**:

`
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(input)
    return output
    
`