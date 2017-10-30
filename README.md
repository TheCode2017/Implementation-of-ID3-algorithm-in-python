# Implementation-of-ID3-algorithm-in-python

following programming languages - Java, Python, C++, Ruby. You cannot use any package or
library for this assignment.
To simplify things, you can assume that the data used to test your implementation will contain
only Boolean (0 or 1) attributes and Boolean (0 or 1) class values. You can assume that there
will be no missing data or attributes. You can also assume that the first row of the dataset will
contain column names and each non-blank line after that will contain a new data instance.
Within these constraints, your program should be able to read and process any dataset
containing any number of attributes. You can assume that the last column would contain the
class labels.
A couple of datasets are provided. You have to build your model using the training dataset,
check the model and prune it with the validation dataset, and test it using the testing dataset.
Below is a summary of the requirements:
• Build a binary decision tree classifier using the ID3 algorithm
• Your program should read three arguments from the command line – complete path of the
training dataset, complete path of the test dataset, and the pruning factor (explained later).
• The datasets can contain any number of Boolean attributes and one Boolean class label. The
class label will always be the last column.
• The first row will define column names and every subsequent non-blank line will contain a
data instance. If there is a blank line, your program should skip it.
• Printing Decision Tree:
Your program should contain a print method that should output the current tree to the
screen. It should be in the following format:
The above tree shows that:
if (wesley = 0 ^ honor = 0 ^ barclay = 0) then class = 1
and also that:
if (wesley = 0 ^ honor = 0 ^ barclay = 1) then class = 0
and also that:
if (wesley = 0 ^ honor = 1 ^ tea = 0) then class = 0
and so on

Some important things and assumptions:
• Remember that entropy uses logarithm of base 2. You should implement log2 and not any
other base. You can assume that log20 = 0.
• After constructing a tree, if you realize that there is a leaf node that contains data from
more than 1 class i.e. it is not a pure node, then you should choose the most frequent class
in that node and output that as the predicted class.
