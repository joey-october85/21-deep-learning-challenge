# 21-deep-learning-challenge
Build a model for a non profitfoundation that will analyze applicant data with the goal of predicting the candidates with the best chances of success to invest in.

## Data Preprocessing

What variable(s) are the target(s) for your model?
- IS_SUCCESSFUL

What variable(s) are the features for your model?
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

What variable(s) should be removed from the input data because they are neither targets nor features?
- EIN
- NAME

## Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
The base model contains 2 Hidden Layers with 80 and 50 nodes respectively and both using "relu" activation. The output layer uses 1 node and the "sigmoid" activation.

#### Were you able to achieve the target model performance?
No.<br>
The final results are as follows<br>
268/268 - 0s - loss: 0.5658 - accuracy: 0.7284 - 486ms/epoch - 2ms/step<br>
Loss: 0.5657624006271362, Accuracy: 0.728396475315094

#### What steps did you take in your attempts to increase model performance?

 - #### Optimization No.01
    - From the base model; an additional hidden layer was created with 30 nodes and "relu" activation
    - Results:<br>268/268 - 1s - loss: 0.5639 - accuracy: 0.7280 - 750ms/epoch - 3ms/step<br>
    Loss: 0.5639129877090454, Accuracy: 0.7280466556549072

- #### Optimization No.02
    - From the base model; Increased epochs to 150
    - Results: <br>
    268/268 - 0s - loss: 0.5650 - accuracy: 0.7275 - 492ms/epoch - 2ms/step<br>
    Loss: 0.5649682879447937, Accuracy: 0.7274635434150696

- #### Optimization No.03
    - From the base model; used "sigmoid" activation in place of "relu"
    - Results: <br>
    268/268 - 1s - loss: 0.5568 - accuracy: 0.7287 - 654ms/epoch - 2ms/step<br>
    Loss: 0.5567643642425537, Accuracy: 0.7287463545799255



### Summary
No significant improvements were achieved with optimization, however, Optimization No.03 is the recommended model as it had the highest accuracy albeit very slightly above the rest of the models.


Jose A Rodriguez Jr<br>
Tutor: Saad Khan