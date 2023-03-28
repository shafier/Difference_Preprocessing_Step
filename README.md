# Difference in Preprocessing step

Whilst analysing Autism dataset, I stumbled onto an alternative way in Preprocessing step. <br>

My curiosity brought me to play around the method, and lo and behold, it works as the common approach <br>

##Steps in the alternative approach##

* dataset
* -> X,  y
* -> preprocessing.fit(X), preprocessing.transform(X) OR preprocessing.fit_transform(X)
* -> split into training (X_train, y_train) and test (X_test, y_test) sets
* -> model.fit(X_train, y_train)
* -> model.predict(X_test) 

##Steps in the common approach##

* dataset
* -> X,y
* -> split into training (X_train, y_train) and test (X_test, y_test) sets
* -> preprocessing.fit(X_train)
* -> preprocessing.transform(X_train)
* -> preprocessing.transform(X_test)
* -> model.fit(X_train, y_train)
* -> model.predict(X_test)

**I am responsible for any error in this analysis. If you spot an error please let me know. I also welcome any feedback. Thank you for your time and attention.** 
> I am reachable at https://www.linkedin.com/in/shafierahim/. Send me a message there. 

