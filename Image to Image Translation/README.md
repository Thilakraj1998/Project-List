<img src="https://www.abtosoftware.com/wp-content/uploads/image3.jpg">

### Image to Image Translation

Image-to-image translation is the process of transforming an image from one domain to another, where the goal is to learn the mapping between an input image and an output image. This task has been generally performed by using a training set of aligned image pairs. However, for many tasks, paired training data will not be available, and to prepare them often takes a lot of work from specialized personnel to obtain thousands of paired image datasets, especially with complex image translations.

It can be applied to a wide range of applications, such as collection style transfer, object transfiguration,season transfer and photo enhancement.

### Implement

The system should perform Text Moderation,

* Develop Python Implementation of Image to Image Translation 
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

In Usage, file creates a function main() accepting  input Image. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be Image URL. if URL is passed then, download the Image file into the local directory
```
def main(input):  
    """
      param1: String : URL to the image file
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks if the string is validate URL and download file into the working directory,uses the downloaded file path else use the simple string text for futher task
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"PATH OF THE SAVED RESULTING IMAGE"}
    
```
### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: Image
output:
  - type: Image
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.