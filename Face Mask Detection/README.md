<img src="https://www.ideas2it.com/wp-content/uploads/2020/09/Facemask-Detection-Blog.jpg" width=1500 height=438>

### Face Mask Detection

The whole world today is facing the COVID-19 pandemic. This situation makes people must adapt to the new normal, for example, working from home, online communication, and keeping clean to reduce the transmission of COVID-19. Moreover, research has found that wearing a mask is one way to reduce the risk of viral transmission. It makes many public places have a measure about their customer must keep a distance between people and wear the face mask correctly. But public service providers are not feasible to thoroughly check whether all a customer wears the mask or not. 


The proposed Implementation should consist of three methods to detect face masks: 
1. Image preprocessing 
2. Face detection and crop 
3. Classification of face masks. 

The system should detect a face mask, not wearing a face mask and incorrect face mask. 

* Develop Python Implementation of Face Mask Detection
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of Face Mask detection module should be saved in respective formats.

The AI Model will help public service providers ensure that all people in this place wear face masks correctly, promote people to use a face mask and ensures that these public places have a safe environment.



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

Input must be either URL to the Image/video. if URL is passed then, download the video file into the local directory, else read from the given path.

```
def main(input=URL):  
    """
      param1: String : URL for the image/video file.

      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks for validate URL and download file into the working directory,uses the downloaded file path.
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"output":"SAVED FILE PATH WITH DETECTION","prediction":{"Mask":Count,"No Mask":Count}]}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  type: image
output:
  type: image
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.

**References**:

1. Johansson MA, Quandelacy TM, Kada S, Prasad PV, Steele M, Brooks JT, et al. SARS-CoV-2 transmission from people without COVID-19 symptoms. JAMA Netw Open. (2021) 4:e2035057. doi: 10.1001/jamanetworkopen.2020.35057

2. Kaur G, Sinha R, Tiwari PK, Yadav SK, Pandey P, Raj R, et al. Face mask recognition system using CNN model. Neurosci Inform. (2021) 2:100035. doi: 10.1016/j.neuri.2021.100035

3. Asghar MZ, Albogamy FR, Al-Rakhami MS, Asghar J, Rahmat MK, Alam MM, Lajis A and Nasir HM (2022) Facial Mask Detection Using Depthwise Separable Convolutional Neural Network Model During COVID-19 Pandemic. Front. Public Health 10:855254. doi: 10.3389/fpubh.2022.855254

