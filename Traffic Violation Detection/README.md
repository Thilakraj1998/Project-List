<img src="https://www.logipix.com/wp-content/uploads/2020/04/vca-measurement.png">

### Traffic Violation Detection

Traffic violation detection systems are practical tools to help traffic administration monitor traffic conditions. It can detect real-time traffic violations like running red lights, speeding, and vehicle retrogress. 

The increasing number of cars in cities can cause a high traffic volume and implies that traffic violations have become more critical nowadays around the world. This causes severe destruction of property and more accidents that may endanger people's lives. Traffic violation detection systems are needed to solve the alarming problem and prevent such unfathomable consequences. The system enforces proper traffic regulations and apprehends those who do not comply. Furthermore, a traffic violation detection system must be realized in real-time as the authorities always track the roads. Hence, traffic enforcers will be at ease in implementing safe streets accurately but also efficiently, as the traffic detection system detects violations faster than humans. 

### Implement

* Implement a AI Model to Detect Traffic Violation in Python.
* Implementation should be able to infer Image and Video from different sources.
* Implementated Model should be easy to integrate with restful API frameworks.


### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/Recognition.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format


### Note

In Usage, file creates a function main() accepting  input video. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.


Input must be either URL to the video. if URL is passed then, download the video file into the local directory, else read from the given path.

```
def main(input=URL):  
    """
      param1: String : URL for the Image/video file.

      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks for validate URL and download file into the working directory,uses the downloaded file path.
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"YES/NO"}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: image/Video
output:
  - type: image/Video
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.