# Introduction:
This project is related to the course  Data-mining for networks of my Master 2 Ubinet. We have tried to implement one algorithm to differentiate between the normal and malicious users of a website. Each user is defined by his IP address and we tried to modelise the behavior of this user by using one graph that summarizes all the flows generated by the user to see if there is a malicious flow associated to his address IP. After defining the kernel function to differenciate between the malicious and the correct users I have used the SVM technique as the classifier that takes the kernel defined before as argument. At the end, I have trained my model and then I evaluate it by using the cross validation to see really the degree of users differenciation that my model can perform.
# Datatsets:
We used the annotated-trace.csv dataset that contains all the informations about the users flows in the website to decide on the types of the users( malicious or correct users).
# experimental Settings:
We build the end host graphlets correspending to flows in annotated-trace.csv then we build the end host models using the random walk kernel and finally we tried to predict the anomalous traffic using the previous built model
# requirements:
 - Pandas
 - Numpy
 - NetworkX to build the graphs with python
# References:
https://www.researchgate.net/publication/220850186_Profiling_the_End_Host
