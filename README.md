# ID3-decision-tree-
### The input is a list of tuples, where each tuple represents a training sample. Each training sample is an (input, class_label) pair, where input is a dictionary of the form attribute: value pairs, and each class_label is either True (representing class C1) or False (representing class C2). An example is given below. This data is about candidates who interviewed for a job and whether or not the candidate was hired. The attributes represent candidate’s level, preferred programming language, whether the candidate is active on Twitter, and whether the candidate has a PhD: 
### training_data = [
### ({'level':'Senior', 'lang':'Java', 'tweets':'no', 'phd':'no'}, False),
### ({'level':'Senior', 'lang':'Java', 'tweets':'no', 'phd':'yes'}, False),
### ({'level':'Mid', 'lang':'Python', 'tweets':'no', 'phd':'no'}, True),
### ({'level':'Junior', 'lang':'Python', 'tweets':'no', 'phd':'no'}, True),
### ({'level':'Junior', 'lang':'R', 'tweets':'yes', 'phd':'no'}, True),
### ({'level':'Junior', 'lang':'R', 'tweets':'yes', 'phd':'yes'}, False),
### ({'level':'Mid', 'lang':'R', 'tweets':'yes', 'phd':'yes'}, True),
### ({'level':'Senior', 'lang':'Python', 'tweets':'no', 'phd':'no'}, False),
### ({'level':'Senior', 'lang':'R', 'tweets':'yes', 'phd':'no'}, True),
### ({'level':'Junior', 'lang':'Python', 'tweets':'yes', 'phd':'no'}, True),
### ({'level':'Senior', 'lang':'Python', 'tweets':'yes', 'phd':'yes'}, True),
### ({'level':'Mid', 'lang':'Python', 'tweets':'no', 'phd':'yes'}, True),
### ({'level':'Mid', 'lang':'Java', 'tweets':'yes', 'phd':'no'}, True),
### ({'level':'Junior', 'lang':'Python', 'tweets':'no', 'phd':'yes'}, False)
### ] 
### Output: the program will construct and output a decision tree (DT) that is built using the training data.define a tree to be one of the following:
### •	True
### •	False
### •	A tuple (attribute, subtree_dict)
### Where True represents a leaf node that returns True (i.e., class C1 or Hire) for any input, False represents a leaf node that returns False (i.e., class C2 or Do not Hire) for any input, and a tuple represents a decision node that, for any input, finds its attribute value, and classifies the input using the corresponding subtree (i.e., this is an internal node with test_attribute attribute).
