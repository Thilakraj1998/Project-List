<img src="https://miro.medium.com/focal/1200/675/34/29/0*KGcqYRXgidCzctW_.jpg">

### Machine Translation

Machine Translation (MT) is the task of automatically converting one natural language into another, preserving the meaning of the input text, and producing fluent text in the output language. While machine translation is one of the oldest subfields of artificial intelligence research, the recent shift towards large-scale empirical techniques has led to very significant improvements in translation quality. 

Most of us were introduced to machine translation when Google came up with the service. But the concept has been around since the middle of last century.

Research work in Machine Translation (MT) started as early as 1950’s, primarily in the United States. These early systems relied on huge bilingual dictionaries, hand-coded rules, and universal principles underlying natural language.

In 1954, IBM held a first ever public demonstration of a machine translation. The system had a pretty small vocabulary of only 250 words and it could translate only 49 hand-picked Russian sentences to English. The number seems minuscule now but the system is widely regarded as an important milestone in the progress of machine translation.

One of the crucial benefits of machine translation is speed as you have noticed that computer programs can translate a huge amount of text rapidly. Yes, the human translator does their work more accurately but they cannot match the speed of the computer.

If you especially train the machine to your requirements, machine translation gives the ideal blend of brisk and cost-effective translations as it is less expensive than using a human translator. With a specially trained machine, MT can catch the setting of full sentences before translating them, which gives you high quality and human-sounding yield. Another benefit of machine translation is its capability to learn important words and reuse them wherever they might fit. 

### Implement

The system should perform Text Translation,

* Develop Python Implementation of Text Translation
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

```
def main(input):  
    """
      param1: String : simple text
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. Accept text/String input from the function.
    #2. perform preprocessing on the data.
    #3. perform prediction/Translation on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction/Translation. for example {"prediction":"TRANSLATED TEXT"}
    
```
### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  type: text
output:
  type: text
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.