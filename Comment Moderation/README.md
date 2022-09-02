<img src="https://www.wpexplorer.com/wp-content/uploads/wordpress-comment-moderation-guide-beginners.jpg" height=425 width=1250>


### Comment Moderation

Comment moderation is essential to growing a digital community. Without comment moderation, you open your community to abuse, profanity and spam—and turn prospective fans and customers away. It’s your responsibility to ensure your brand environment is safe and inviting to your audience. Moderating online communities while encouraging engagement is the most failproof way to achieve this.

Moderation is key to encouraging, not stifling, conversation. You want fans to feel that they can contribute in a valuable way by building an environment that facilitates spirited debate and respectful discussion. This spurs your community’s growth and in turn encourages brand evangelism. Closing comments is never an option; in fact, your community gives you a competitive edge because, unlike products, communities can’t be replicated so easily.

Comment Moderation is the type of Text Classification problem where the model must be trained on different action verbs to everyday slang used over the internet to identify which comment is harmful to the other user/community.

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

`
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(input)
    return output
    
`