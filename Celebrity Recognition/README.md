<img src="https://static.us-east-1.prod.workshops.aws/public/9a8e846d-8d8a-4769-ac9b-805a066609ba/static/images/celebrity.jpg" width=1500 height=438>

### Celebrity Recognition



To make it easy for customers to automatically recognize tens of thousands of well-known personalities in images and videos using machine learning. For example, in social media or news and entertainment industries where information gathering can be time critical, you can use this operation to identify celebrities in an image, and return links to celebrity webpages/Social Media Accounts, if they're available.


### Implement

Since Face Detection Problem has a wide variety of applicable Application in different domain and industries

* Develop Python Implementation of Celebrity Recognition
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of elebrity Recognition module should be saved in respective formats.

### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/Recognition.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format

### Note

In Usage, file creates a function main() accepting single input, which can either be an image or video. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

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
    #4. return output :output must be a json, which included output prediction. for example {"output":"SAVED FILE PATH WITH DETECTION/Recognition","prediction":[List of Detected Celebrity Names]]}
    
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
**saved by name : blobcity.yaml**

Also include requirement.txt file in the submission with required version of the library mentioned in it.