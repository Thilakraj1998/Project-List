<img src="https://enhancebusinesssolutions.com/wp-content/uploads/2019/09/broadcast-broadcasting-camcorder-66134-3.jpg" height=425 width=1300>

### Video Moderation 

The daily volume of User Generated Content (UGC) and third-party content has been increasing substantially in industries like social media, e-commerce, online advertising, and photo sharing. Customers often want to review this content to ensure that their end-users are not exposed to potentially inappropriate or offensive material, such as nudity, violence, drug use, adult products, or disturbing images. In addition, broadcast and Video-On-Demand (VOD) media companies may be required to ensure that the content they create or license carries appropriate ratings as per compliance guidelines for various geographies or target audiences. Today, many companies employ teams of human moderators to review content, while others simply react to user complaints to take down offensive images, ads, or videos. However, human moderators alone cannot scale to meet these needs at sufficient quality or speed, leading to a poor user experience, high costs to achieve scale, or even a loss of brand reputation.


The system should be able to classification Video content impacts/type,

* Develop Python Implementation of Video Moderation using AI/ML technique
* Implementation should have the ability to infer video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.

### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/Recognition.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format

### Note

In Usage, file creates a function main() accepting single input video. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be either URL to the video. if URL is passed then, download the video file into the local directory, else read from the given path.

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
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"abusive"}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  type: video
output:
  type: label
requirement: requirement.txt
main: main.ipynb
```
**saved by name : blobcity.yaml**

Also include requirement.txt file in the submission with required version of the library mentioned in it.