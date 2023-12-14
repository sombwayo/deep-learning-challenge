Overview:
The nonprofit foundation Alphabet Soup wanted a tool to help them select applicants for funding. They need a binary classifier to predict whether applicants will be successful if funded by Alphabet Soup.


Data Preprocessing:

Unnecessary metrics such as EIN and Name were removed from the dataset and all remaining metrics were considered in the model. Both Classification and Application Type were features of the model.
•	What variable(s) are the target(s) for your model? The target variable is the "IS_SUCCESSFUL" column from application_df
•	What variable(s) are the features for your model? The features variable is every other column from application_df, which was done by dropping the
"IS_SUCCESSFUL" column from the original dataframe.
•	What variable(s) should be removed from the input data because they are neither targets nor features? The "EIN" and "NAME" columns were dropped because they were neither targets nor features for the dataset.
Compiling, Training, and Evaluating the Model:
1.	How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the first attempt, I added two layers ( layer 1: 8 neurons; layer 2: 5 neurons). Both
layers were activated-by the rectified linear unit (ReLu).There were no particular selection criteria for the neural networks parameters and the neurons in each later were random guesses from which to iterate upon in the second try.
2.	Were you able to achieve the target model performance? - I was not able to achieve the 75% model accuracy target

3.	What steps did you take in your attempts to increase model performance?
•	Removed more column (EIN, NAME, STATUS, ASK_AMT (newly removed))
•	In all attempts, adjusted neurons in each of the LAYERS
•	In the last two attempts, added an additional layer making three layers with in an attempt to achieve higher model accuracy.
•	In the last attempt, changed the epoch from 100 to 150.
