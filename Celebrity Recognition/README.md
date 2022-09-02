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

**Example**:

`
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(input)
    return output
    
`