<img src="https://editor.analyticsvidhya.com/uploads/13629post.JPG">

### Image Super Resolution

Image super-resolution (SR) is the process of recovering high-resolution (HR) images from low-resolution (LR) images. It is an important class of image processing techniques in computer vision and image processing and enjoys a wide range of real-world applications, such as medical imaging, satellite imaging, surveillance and security, astronomical imaging, amongst others.

With the advancement in deep learning techniques in recent years, deep learning-based SR models have been actively explored and often achieve state-of-the-art performance on various benchmarks of SR. A variety of deep learning methods have been applied to solve SR tasks, ranging from the early Convolutional Neural Networks (CNN) based method to recent promising Generative Adversarial Nets based SR approaches.

Image super-resolution (SR) problem, particularly single image super-resolution (SISR), has gained a lot of attention in the research community. SISR aims to reconstruct a high-resolution image ISR from a single low-resolution image ILR. Generally, the relationship between ILR and the original high-resolution image IHR can vary depending on the situation. Many studies assume that ILR is a bicubic downsampled version of IHR, but other degrading factors such as blur, decimation, or noise can also be considered for practical applications.

### Implement

The system should perform Text Moderation,

* Develop Python Implementation of Image Super Resolution Model
* Implementation should have the ability to infer diiferent level of Image quality and produce desired High Resolution images.
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

In Usage, file creates a function main() accepting  input Image file URL. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

Input must be either single Image input or URL to the Image. if URL is passed then, download the Image file into the local directory
```
def main(input):  
    """
      param1: String : URL
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks if the string is validate URL and download the image file into the working directory,uses the downloaded file path for further prediction/Procedures.
    #2. perform preprocessing on the data.
    #3. perform AI Super Resolution on the given data and produce respective output and save the image
    #4. return output :output must be a json, which included output prediction. for example {"prediction":"PATH TO THE SAVED OUTPUT IMAGE"}
    
```
### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  type: Image
output:
  type: Image
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.