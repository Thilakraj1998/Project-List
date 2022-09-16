<img src="https://chisw.com/wp-content/uploads/2022/06/the-most-popular-nlg-use-cases1.jpg">

### Text Generation


Text generation is a subfield of natural language processing (NLP).Text generation is the task of generating text with the goal of appearing indistinguishable to human-written text. This task if more formally known as "natural language generation" in the literature.

Text generation can be addressed with Markov processes or deep generative models like LSTMs. Recently, some of the most advanced methods for text generation include BART, GPT and other GAN-based approaches. Text generation systems are evaluated either through human ratings or automatic evaluation metrics like METEOR, ROUGE, and BLEU.

### Applications

1. NLG is used by businesses in a variety of industries to generate reports. Data may be analyzed to obtain actionable insights and then converted into accessible reports using NLG-powered Business Intelligence solutions. 

2. By stringing long sequences of phrases together and creating personalized content, NLG can be utilized to automate content generation. 

3. For performance reporting, the banking industry heavily relies on data and insights. NLG systems can also be used to automate profit and loss reports. 

### Implement

The system should perform Text Moderation,

* Develop Python Implementation of Text Generation
* Implementation should have the ability to infer different level of text sensitivity or multilingual.
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

In Usage, file creates a function main() accepting  input text. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be either single text input or URL to the textfile. if URL is passed then, download the text file into the local directory
```
def main(input):  
    """
      param1: String : URL or simple text
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks if the string is validate URL and download file into the working directory,uses the downloaded file path.else use the simple string text for futher task
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"prediction":OutCome}
    
```
### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: text
output:
  - type: Text
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.