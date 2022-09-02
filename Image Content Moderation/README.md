<img src="https://influencermarketinghub.com/wp-content/uploads/2022/05/op-Content-Moderation-tools-for-2022.png" width=1500 height=438>

### Image Moderation

The daily volume of User Generated Content (UGC) and third-party content has been increasing substantially in industries like social media, e-commerce, online advertising, and photo sharing. Customers often want to review this content to ensure that their end-users are not exposed to potentially inappropriate or offensive material, such as nudity, violence, drug use, adult products, or disturbing images. In addition, broadcast and Video-On-Demand (VOD) media companies may be required to ensure that the content they create or license carries appropriate ratings as per compliance guidelines for various geographies or target audiences. Today, many companies employ teams of human moderators to review content, while others simply react to user complaints to take down offensive images, ads, or videos. However, human moderators alone cannot scale to meet these needs at sufficient quality or speed, leading to a poor user experience, high costs to achieve scale, or even a loss of brand reputation.


The system should be able to classification Image content impacts/type,

* Develop Python Implementation of Image Moderation using AI/ML technique
* Implementation should have the ability to infer Image files.
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

In Usage, file creates a function main() accepting single input, which can either be an image or video. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

**Example**:
```
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(data)
    return output
    
```