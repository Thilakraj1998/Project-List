<img src="https://newmediaservices.com.au/wp-content/uploads/2019/02/Types-of-Text-Moderation.png">

### Text Moderation

Text moderation is the process of blocking, approving or reviewing content submissions based on the policies and thresholds of a certain site.  This type of content moderation is used to enhance human moderation in an environment that require partners, employees and consumers who can generate text content.

This includes blog or forum comments, reviews, chat rooms, discussions boards and tweets. The main goal is to protect your users and brand without affecting user experience. Before determining if your business needs text moderation, it is important to look at your current metrics and the volume of your UGC. 

### Types of Text Moderation

This types of text moderation can be used to deal with all kinds of user-generated content to keep your online community safe and user-friendly.

* Chat Moderation :- This process is the monitoring and moderating of live chat sessions to prevent policy violations of users. Its coverage includes webcam sessions and simple chat sessions.

* Comment and Post Moderation:- Moderators will review each and every comment and post content submitted by users in online communities. The checking of content is done in real-time.

* Tweet Moderation:-Since Twitter has taken huge part on social media platform, it is essential that moderating what audiences have to voice out about brands. Particularly, when people share about user experience and impressions on a business’ products and services, keeping track of all these tweets helps control how it can affect the business’ reputation, positively or negatively

* Review Moderation:-People can post negative reviews about certain products or services. At times, the reviews may not even be true. A negative review has numerous impacts on brands if left unattended. Review moderation manages user reviews to protect your brand reputation by scrutinizing between authentic accounts of user experience from fabricated stories about availing the brand’s services

* Social Media Moderation:-Most brands are using social media to engage with their users and site visitors, making it an absolute necessity to effectively manage user-generated content across social platforms. Moderation services for social media efficiently manage and moderate user submissions to help spread a positive online presence and influence.

**Importance of Text Moderation**

People use all sorts of abbreviations, slangs, grammatically incorrect sentences, uncommon words, words not found in Oxford dictionary, and what not? At the same time, these Text many times carry vital information that could be very useful to you even in saving somebody's precious life.

Content that tarnishes a platform or a brand’s reputation can take various forms, but the most rudimentary format that can easily permeate through media is text. Even seemingly random words, when placed in a particular order, can create enough chaos to topple a brand. That’s the power of text – be it a blog article, a comment, or a file from a text bin. 

The problem that we are trying to solve is essentially a text classification problem.

### Implement

The system should perform Text Moderation,

* Develop Python Implementation of Text Moderation
* Implementation should have the ability to infer diiferent level of text sensitivity or multilingual.
* Implementation should be easy to integrate with restful API frameworks.

### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction.
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
    #1. checks if the string is validate URL and download file into the working directory,uses the downloaded file path.else use the simple string text for further task
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"MOderation Result"}
    
```
### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: text/text.txt
output:
  - type: label/class
main: main.ipynb
```