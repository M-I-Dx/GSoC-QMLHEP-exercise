# GSoC-QMLHEP-exercise
Solution of GSoC QMLHEP exercise

## Machine Learning part

(Data was in a bit weird format so I converted it into an excel file through Libre Office.)

The following files constitute of the solution of the ML problem. 
```
GSoC CERN ML.ipynb
GSoC CERN SVM.ipynb
```
The first .ipynb (GSoC CERN ML.ipynb) file shows the implementation of the following traditional ML models:
1. k-Nearest Neighbor
2. Naïve Bayes
3. Logistic Regression
4. Support Vector Machines
5. Decision Trees
6. Random Forests
7. Multi-layer Perceptrons

Deep-Learning model with the following architecture and configuration was also used on the same dataset.
```
model_deeplearning = keras.Sequential([
    keras.layers.Flatten(input_shape=(5,)),
    keras.layers.Dense(16, activation=tf.nn.relu),
    keras.layers.Dense(16, activation=tf.nn.relu),
    keras.layers.Dense(1, activation=tf.nn.sigmoid),
])

model_deeplearning.compile(optimizer='sgd',
              loss='binary_crossentropy',
              metrics=['accuracy'])
```

The conclusion of the evaluation of these models was that Logistioc Regression, SVM and Multi-layer Perceptron outperformed every other model including the Deep-learning model. Out of these three models SVM is my choise. 
In the second .ipynb file (GSoC CERN SVM.ipynb) the SVM Model is evaluated extensively on other preformance matrices like ROC. 

#### Conclusion: It's not who has the best algorithm that win. It's who has the most data.

### Quantum Computing Part

The following file constitutes the solution of the Quantum Computing problem.
```
GSoC CERN QC.ipynb
```

(Sorry you will have to scroll down a lot because th plot the graph of the rotation vs the probability of measuring the state in the |0⟩ state was plotted on 10000 data points with an increment of 0.1 degree to get best results)

