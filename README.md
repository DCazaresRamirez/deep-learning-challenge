<h1>Neural Network Model Report</h1>

  <div class="section">
        <h2>Overview of the Analysis</h2>
        <p>The purpose of this analysis was to develop a neural network model to predict the success of funding applications for Alphabet Soup. The goal was to use features from the provided dataset to classify applications as successful or not, and to optimize the model to achieve the best predictive accuracy possible.</p>
    </div>

  <div class="section">
        <h2>Results</h2>
        
  <h3>Data Preprocessing</h3>
        <ul>
            <li><strong>Target Variable:</strong> The target variable for the model is <code>IS_SUCCESSFUL</code>.</li>
            <li><strong>Features:</strong> The features used for the model include <code>APPLICATION_TYPE</code>, <code>AFFILIATION</code>, <code>CLASSIFICATION</code>, <code>USE_CASE</code>, <code>ORGANIZATION</code>, <code>STATUS</code>, <code>INCOME_AMT</code>, and <code>SPECIAL_CONSIDERATIONS</code>.</li>
            <li><strong>Variables to Remove:</strong> The variables <code>EIN</code> and <code>NAME</code> were removed from the dataset as they were non-beneficial ID columns that did not contribute to the model's predictive power.</li>
        </ul>

  <h3>Compiling, Training, and Evaluating the Model</h3>
        <ul>
            <li><strong>Neurons, Layers, and Activation Functions:</strong> The neural network model was designed with three hidden layers. The architecture included:
                <ul>
                    <li>First hidden layer with 128 neurons and ReLU activation function</li>
                    <li>Second hidden layer with 64 neurons and ReLU activation function</li>
                    <li>Third hidden layer with 32 neurons and ReLU activation function</li>
                    <li>Dropout layer with a rate of 0.5 to reduce overfitting</li>
                    <li>Output layer with 1 neuron and a sigmoid activation function for binary classification</li>
                </ul>
            </li>
            <li><strong>Target Model Performance:</strong> The highest achieved accuracy was 72.9%, which is below the target of 75%.</li>
            <li><strong>Steps Taken to Increase Model Performance:</strong> To optimize the model, several strategies were employed:
                <ul>
                    <li>Added more neurons to the hidden layers</li>
                    <li>Included additional hidden layers</li>
                    <li>Applied dropout regularization</li>
                    <li>Utilized early stopping to prevent overfitting</li>
                    <li>Adjusted the learning rate and increased the number of epochs</li>
                </ul>
            </li>
        </ul>
    </div>

  <div class="section">
        <h2>Summary</h2>
        <p>In summary, the deep learning model for predicting funding success achieved an accuracy of 72.9%. Despite implementing various optimization techniques, the target accuracy of 75% was not met. The adjustments made included modifying the model architecture, using dropout, and changing the training regimen.</p>
