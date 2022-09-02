
<img src="https://miro.medium.com/max/1200/1*TWZM67eaCs0mMBFqs9HFBA.jpeg" height=450 width =1500>

### Car Number Plate Detection and Optical Character Recognition(OCR)

The massive integration of information technologies, under different aspects of the modern world, has led to the treatment of vehicles as conceptual resources in information systems. Since an autonomous information system has no meaning without any data, there is a need to reform vehicle information between reality and the information system. This can be achieved by human agents or by special intelligent equipment that will allow the identification of vehicles by their registration plates in real environments. Among intelligent equipment, mention is made of the system of detection and recognition of the number plates of vehicles. The system of vehicle number plate detection and recognition is used to detect the plates and then make the recognition of the plate that is to extract the text from an image and all that thanks to the calculation modules that use location algorithms, segmentation plate and character recognition. The detection and reading of license plates is a kind of intelligent system and it is considered because of the potential applications in several sectors which are quoted:

- Command force: This system is used for the detection of stolen and searched vehicles. The detected plates are compared to those of the reported vehicles.

- Parking management: The management of car entrances and exits.

- Road safety: This system is used to detect license plates exceeding a certain speed, coupling the plate reading system with road radar, crossing wildfires


### Implement

Since Car Number/License Plate Detection Problem has a wide variety of applicable Application in different domain and industries

* Develop Python Implementation of the follow problem to Detection and recognize License Plate Number
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of detection module should be saved in respective formats.


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

```
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(data)
    return output
    
```