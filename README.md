# Challenge21_JuanJCoronado

The Jupyternotebook has been attached. Also, ahead is the summary:

1. Overview of the analysis: Explain the purpose of this analysis
The purpose of this analysis is to create a neural network in order to make predictions based on new test data. The model learns on testing information, which was splitted using test_train. Also, there was a data pre processing section, where certain columns were removed, the data was scaled, and the data was manipulated to be on a categorical format. Finally, there were three different models used with different combinations of layers/neurons/activations/epochs.


2. Results: Using bulleted lists and images to support your answers, address the following questions:
* Data Preprocessing
    * What variable(s) are the target(s) for your model? IS_SUCCESSFUL
    * What variable(s) are the features for your model? All other variables that are not IS_SUCCESSFUL
    * What variable(s) should be removed from the input data because they are neither targets nor features? EIN and NAME
* Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
        * I created 3 differrent models, First with 3 layers (relu) and an output (sigmoid) layer. 20, 15, and 15 neurons for each and 10 epochs.
        * Second with 4 layers (3 relu and 1 tanh) and an output (sigmoid) layer. 80, 30, 30, and 25 neurons for each and 100 epochs.
        * Third with 5 layers (4 relu and 1 tanh) and an output (sigmoid) layer. 150, 120, 100, 100, and 80 neurons for each and 150 epochs.
        * These were all selected to check if the accuracy for the model would go up. In some cases it did go up, but it’s commonly ~73% accuracy approximately.
    * Were you able to achieve the target model performance? no, it was not able to reach 75% but it was very close to this number.
    * What steps did you take in your attempts to increase model performance?
        * I tried increasing the number of layers, switching some layers to activation method tanh instead of relu, increasing the number of neurons, and also increasing the number of epochs,            all of these to see if performance would increase.


3. Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
As I mentioned, I created 3 models to see which had higher accuracy. All of them has very close accuracy levels, at around 35%. There are many different models available, each with its own strengths and weaknesses. Perhaps a good model to also try would be Random Forests fue to their scalability, robustness, and interpretability.
