# deep-learning-challenge
Module 21 Challenge


Overview of the Analysis: The purpose of this analysis was to develop a deep learning model to predict the success of funding applications for Alphabet Soup. The model aimed to accurately classify whether an organization would be successful in receiving funding based on various features provided in the dataset.
Results:
Data Preprocessing:
• Target Variable: The target variable for the model was the IS_SUCCESSFUL column.
• Features: The features used for the model were the rest of the columns without the IS_SUCCESSFUL column.
• Variables to Remove: The variables that needed to be removed from the input data because they are neither targets nor features were EIN and NAME.

Compiling, Training, and Evaluating the Model:
• Neurons, Layers, and Activation Functions: The original attempt at the neural network (nn) consisted of two hidden layers with 80 and 30 neurons respectively, both using the ReLU activation function. The output layer had 1 neuron with a sigmoid activation function. 
• Target Model Performance: The target model performance was 75% accuracy. The accuracy achieved by the original attempt (nn) was reported as 0.7274.
• Attempts to Increase Model Performance:
1. Optimization Attempt 1 (nn1): This attempt involved dropping two additional columns, creating more bins for rare occurrences in columns, and resulted in an accuracy of 0.7289.
2. Optimization Attempt 2 (nn2): This attempt included adding more neurons to the first and second hidden layers, as well as adding an additional hidden layer. However, the accuracy achieved was 0.7273, indicating no significant improvement.
3. Optimization Attempt 3 (nn3): This attempt involved using the ReLU activation function on all layers and increasing the number of epochs to 150. The accuracy obtained was 0.7232.

Summary: The deep learning model achieved an accuracy of approximately 0.7274 in its original form. Optimization attempts were made to improve the model's performance, including modifying the input data and neural network architecture. However, these attempts resulted in only marginal improvements or slight decreases in accuracy.
For solving this classification problem, a recommendation would be to explore other models apart from deep learning. Decision trees, random forests, or gradient boosting algorithms could be potential alternatives to consider. These models have shown success in classification tasks and may provide better performance for the given dataset. Further experimentation with different models and hyperparameter tuning can lead to more accurate predictions.