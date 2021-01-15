# GameOSTClassifier
Soundtrack classification of several game soundtracks. I has some game soundtracks on my desktop and decided to do something fun with them

# The Labels: 

Zelda - Ocarina of Time
Hades 
Kingdom Hearts
Persona5 Royal
Hollow Knight
Witcher 3 - Blood and Wine

Each game soundtrack contains 10 songs. Each track had to be cut to 30 seconds, I used pydub. 
Each track was then cut into 3 second segments, and mfccs were extracted using Librosa library.

The model was overfitting, with 98% accuracy for training set, but ~ 60% for validation. So needed to fix the overfitting using Dropout() and Regularization l2.

The algorithm performs just OK, with roughly 68% accuracy. 

At the end of the code I plot the loss and error to see if the gap was minimized, And finally performed a confusion matrix
and calculated the accuracy myself. 

Im sure it can be improved, please contact me if you have any suggestions
