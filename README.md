# HandwrittenDigitRecognitionWithoutDeepLearning

initially, we used a dataset that includes images with numbers written by hand and our main purpose is to Use a model that recognizes numbers them. The model we will use is a neural one network with the scratch method and the use of mathematical functions which we will need for the successful prediction. At the beginning of it program, we will import all the necessary libraries that will we need to get the desired result and we will we also import our data set. With the command our figure shows All the columns and tuples that our dataset has, with the command head will show us the first tuples and with the command tail(10) it will show us the last 10 tuples. Then we'll split up the data from the data set in a random fashion using the random.shuffle command and we will set variables for the data that we will train and test. Next year, I will use mathematical functions with the main purpose of extract the result we desire as our model will it has a simple two-tier architecture. The input layer a[0] will has 784 units corresponding to 784 pixels in each input image
28x28. A hidden layer a[1] that has 10 units with activation ReLU, and finally our output layer a[2] which has 10 units which correspond to the ten-digit categories with softmax activation. Now for our model's prediction of what number
it is illustrated that we will make the following types:
For ForwardPropagation:
 Variable_Function_Z^[1]=Variable_Function_W^[1]
Variable_Function_ X+ Variable_Function_ b^[1]
 Variable_Function_ A^[1]=gReLU(Variable_Function_ Z^[1]))
 Variable_Function_ Z^[2]= Variable_Function_ W^[2]
Variable_Function_ A^[1]+ Variable_Function_ b^[2]
 Variable_Function_ A^[2]=gsoftmax(Variable_Function_ Z^[2])
For BackwardPropagation:
 digits_ Z^[2]= Variable_Function_ A^[2]− OneHot_Variable_Y
 digits_ W^[2]=(1/m) digits_ Z^[2] Variable_Function_ A^([1]T)
 digits_ B^[2]=(1/m)Σ digits_ Z^[2]
 digits_Z^[1]= Variable_Function_W^([2]T) digits_Z^[2].∗g[1]′(
Variable_Function_z^[1])
 digits_ W^[1]=(1/m) digits_ Z^[1] Variable_Function_ A^([0]T)
 digits_ B^[1]=(1/m)Σ digits_ Z^[1]
For Parameter Updates:
 Variable_Function_ W^[2]:= Variable_Function_ W^[2]−th digits_
W^[2]
 Variable_Function_ b^[2]:= Variable_Function_ b^[2]−α digits_
b^[2]
 Variable_Function_ W^[1]:= Variable_Function_ W^[1]−th digits_
E^[1]
 Variable_Function_ b^[1]:= Variable_Function_ b^[1]−α digits_
b^[1]
For the variables and shapes in ForwardPropagation:
Variable_Function_ A^[0]= Variable_Function_ X: 784 x m
Variable_Function_ Z^[1]∼ Variable_Function_ A^[1]: 10 x m
Variable_Function_ W^[1]: 10 x 784 (as Variable_Function_ W^[1]
Variable_Function_ A^[0]∼ Variable_Function_ Z^[1])
Variable_Function_ B^[1]: 10 x 1
Variable_Function_ Z^[2]∼ Variable_Function_ A^[2]: 10 x m
Variable_Function_ W^[1]: 10 x 10 (as Variable_Function_ W^[2]
Variable_Function_ A^[1]∼ Variable_Function_ Z^[2])
Variable_Function_ B^[2]: 10 x 1
For the variables and shapes in BackwardPropagation:
 digits_ z^[2]: 10 x m (Variable_Function_ A^[2])
 digits_ W^[2]: 10 x 10
 digits_ B^[2]: 10 x 1
 digits_ Z^[1]: 10 x m (Variable_Function_ A^[1])
 digits_ W^[1]: 10 x 10
 digits_ B^[1]: 10 x 1
Next in our program we will create functions that will make the prediction and give us the accuracy who have. Next, we'll create two more functions where in the first one that takes the variables from the data set i.e pictures with the numbers and the second one will make the prediction function will do the test using the special variables that we have set to do the test. Finally we will display them images with the numbers randomly and that shows us the prediction which has done our model and below the number that will the image depicts and then we will see the accuracy you have it our program depending on the set with the numbers chosen by the our model from the dataset.
