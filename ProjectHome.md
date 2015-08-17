This is a small library that can train Restricted Boltzmann Machines, and also Deep Belief Networks of stacked RBM's.

Train RBM's:
```
%train an RBM with binary visible units and 500 binary hidden
model= rbmBB(data, 500);

%visualize the learned weights
visualize(model.W);
```

Do classification:
```
model= rbmFit(data, 500, labels);
prediction= rbmPredict(model, testdata);
```

Train a Deep Belief Network with 500,500,2000 architecture for classification:
```
models= dbnFit(data, [500 500 2000], labels);
prediction= dbnPredict(models, testdata);
```

see included example code for more

I can be contacted on andrej.karpathy@ gmail.




**NOTE:**
This was a class project that I worked on for 1 month and then abandoned development for almost 4 years ago. Please do not send me specific questions about issues with the code or questions on how to do something. I only put this code online in hope that it can be useful to others but cannot fully support it.

If you would like pointers to more actively maintained implementations, have a look here (https://github.com/rasmusbergpalm/DeepLearnToolbox) or maybe here (https://github.com/lisa-lab/DeepLearningTutorials)

Sorry and best of luck!