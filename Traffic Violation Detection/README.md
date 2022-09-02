<img src="https://www.logipix.com/wp-content/uploads/2020/04/vca-measurement.png">

### Traffic Violation Detection

Traffic violation detection systems are practical tools to help traffic administration monitor traffic conditions. It can detect real-time traffic violations like running red lights, speeding, and vehicle retrogress. 

The increasing number of cars in cities can cause a high traffic volume and implies that traffic violations have become more critical nowadays around the world. This causes severe destruction of property and more accidents that may endanger people's lives. Traffic violation detection systems are needed to solve the alarming problem and prevent such unfathomable consequences. The system enforces proper traffic regulations and apprehends those who do not comply. Furthermore, a traffic violation detection system must be realized in real-time as the authorities always track the roads. Hence, traffic enforcers will be at ease in implementing safe streets accurately but also efficiently, as the traffic detection system detects violations faster than humans. 

### Implement

* Implement a AI Model to Detect Traffic Violation in Python.
* Implementation should be able to infer Image and Video from different sources.
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

In Usage, file creates a function main() accepting  input video. Through this function, other required functions to make detection/prediction should be called and return output in the appropriate format.

**Example**:

```
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(input)
    return output
    
```