<img src="https://miro.medium.com/max/1400/1*YiWMus7TRTugrljVyTeCZw.jpeg">

### AI Generated Arts

A new field of digital art is stretching the boundaries of creativity and disrupting how art is made. Artists build autonomous robots to collaborate with, feed algorithms with data, and train machines to generate novel visual works. They work with computer programs that mimic the human mind to generate a never-ending stream of unique artworks. Artificial intelligence has emerged as a desirable collaborator in artistic creation.

AI artists embrace the interplay between accident and control and use AI to find a balance between the two while developing novel concepts and visuals. 


It offers immense benefits such as
–Ensuring the generation of higher quality outputs by self-learning from every set of data.

- Lowering the risks associated with a project

- Training reinforced machine learning models to be less biased

- Enabling depth prediction without sensors

- Enabling localization and regionalization of content via deepfakes

- Allowing robots to comprehend more abstract concepts both in simulation and the real world.

### Implement

* Implement a AI art Generator python model to create unique arts.
* The implementation should be able to infer unique images for each invocation.
* Implementated Model should be easy to integrate with restful API frameworks.


### Usage

* Create a separate ipynb file required for model prediction/Generation and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make the art generation.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/generation.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format

### Note

In Usage, file creates a function main(). Through this function, other required functions to make generation should be called and return output in the appropriate format.

```
def main():  
    """
      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. perform generation of the art using the generator model
    #2. return output :output must be a json, which included path of the generated image in the working directory. for example {"output":"SAVED FILE PATH OF GENERATED ART"}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1

output:
  type: image
requirement: requirement.txt
main: main.ipynb
```

Also include requirement.txt file in the submission with required version of the library mentioned in it.
