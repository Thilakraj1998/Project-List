<img src="https://i0.wp.com/turbolab.in/wp-content/uploads/2021/09/Text-Summarization-NLP.jpg?fit=1000%2C579&ssl=1">

### Text Summarization

Text summarization is the technique for generating a concise and precise summary of voluminous texts while focusing on the sections that convey useful information, and without losing the overall meaning.
Automatic text summarization aims to transform lengthy documents into shortened versions, something which could be difficult and costly to undertake if done manually.
Machine learning algorithms can be trained to comprehend documents and identify the sections that convey important facts and information before producing the required summarized texts. 

With the present explosion of data circulating the digital space, which is mostly non-structured textual data, there is a need to develop automatic text summarization tools that allow people to get insights from them easily. Currently, we enjoy quick access to enormous amounts of information. However, most of this information is redundant, insignificant, and may not convey the intended meaning. For example, if you are looking for specific information from an online news article, you may have to dig through its content and spend a lot of time weeding out the unnecessary stuff before getting the information you want. Therefore, using automatic text summarizers capable of extracting useful information that leaves out inessential and insignificant data is becoming vital. Implementing summarization can enhance the readability of documents, reduce the time spent in researching for information, and allow for more information to be fitted in a particular area.

### Implement

The system should perform Text Summerization,

* Develop Python Implementation of Text Summarization
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

In Usage, file creates a function main() accepting  input text file URL. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be either single text file input or URL to the text file. if URL is passed then, download the text file into the local directory
```
def main(input):  
    """
      param1: String : URL or simple text
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks if the string is validate URL and download file into the working directory,uses the downloaded file path.else use the simple string text for futher task
    #2. perform preprocessing on the data.
    #3. perform prediction/Summarization on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction/Summarization. for example {"prediction":"Summary"}
    
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
  - type: text
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.