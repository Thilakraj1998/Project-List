<img src="https://www.freecodecamp.org/news/content/images/2020/09/wall-5.jpeg">

### Sentiment Prediction/Analysis

Sentiment analysis is contextual mining of text which identifies and extracts subjective information in source material, and helping a business to understand the social sentiment of their brand, product or service while monitoring online conversations.

With the recent advances in deep learning, the ability of algorithms to analyse text has improved considerably. 

In essence, the sentiment analysis application brings additional flexibility and insight into the presentation of the brand and its products. It allows companies to:

1. track the perception of the brand by the customers;
2. point out the specific details about the attitude;
3. Find patterns and trends;
4. keep a close eye on the presentation by the influencers.

All this allows us to adjust to the state of things accordingly and give the product a proper presentation.

Overall, sentiment analysis can be used to:

1. Automate media monitoring process and the accompanying alert system
2. Monitor mentions or reviews of the brand on different platforms (blogs, social media, review sites, forums, etc.)
3.Categorize urgency of mentions according to the relevancy scoring (i.e., which platform, type of user is vital to the brand)



### Implement

* Implement and train Sentiment Analysis Model in python using AI/ML technique.
* Implemented Model should be able to classify comment properly.
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

In Usage, file creates a function main() accepting  input text. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be simple text input or URL to the textfile. if URL is passed then, download the video file into the local directory

```
def main(input=URL):  
    """
      param1: String : Simple text or text file URL

      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks for validate URL and download file into the working directory,uses the downloaded file path.
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"sentiment type"}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: text/text files
output:
  - type: boolean/label
main: main.ipynb
```
