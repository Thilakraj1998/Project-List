<img src="https://miro.medium.com/max/1400/1*Fm58r_RQ53sEHfwFa28LpA.png">

### Spam Moderation

Spam moderation is a program used to detect unsolicited, unwanted, and virus-infected emails and prevent those messages from getting into a user's inbox. Like other types of filtering programs, a spam filter looks for specific criteria on which to base its judgments.

Internet service providers, free online email services, and businesses use email filtering tools to reduce the spam distribution risk. For example, one of the simplest and earliest versions of spam filtering, like the one that Microsoft's Hotmail used, was set to watch out for particular words in the subject lines of messages. An email was excluded from the user's inbox whenever the filter recognized one of the specified words.

This method is not especially effective and often omits legitimate messages, called "false positives," while letting actual spam messages through.



### Implement

* Implement and train Comment Moderation Model in python using AI/ML technique.
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

**Example**:

```
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(input)
    return output
    
```  
