# Which_attributes_in_the_dataset_are_important ?

Focus : If we have a large dataset , sometime's we find it difficult to select which attributes work poorly and affected the accuracy. 

Pre-require : Basic knowlodge of ML.

We use a famous tool for data mining Call "Weka"

Weka : https://www.cs.waikato.ac.nz/ml/weka/

Download : https://sourceforge.net/projects/weka/

Data-set : UCI data repository

I show you with a example how to do that.

First, take the diabetes dataset from my repository.

It contain :

1. Number of times pregnant

2. Plasma glucose concentration a 2 hours in an oral glucose tolerance test

3. Diastolic blood pressure (mm Hg)

4. Triceps skin fold thickness (mm)

5. 2-Hour serum insulin (mu U/ml)

6. Body mass index (weight in kg/(height in m)^2)

7. Diabetes pedigree function

8. Age (years)

9. Class variable (0 or 1)


Open Weka and click the Explorer button. 

Then onen the diabetes data set by clicking on open file.

Now you can see all the attributes(total 9) of this dataset.

If you click Visuallize all, you see the graph of all attributes by their class.

If you look closely, you see that pregnancy is not a good feature for run machine learning algorithm.

There are some other.


So, We use Filter.

Click On : Filter -> choose -> supervised -> AttributeSelection 

Then Again Click on the white box where AttributeSelection is shown.

This will open a new window.

Then go to evaluator and choose : cfsSubsetEval

For search choose : GreedyStepWise

Then press Ok. Now If you Press Apply button this will give you whice attributes Subset are important and remove whice are not.

In my diabetes dataset :

1. Plasma glucose.

2. Body mass

3. Diabetes pedigree function

4. Age.



You can use Weka in to classify the dataset by different build in algorithm. One main advantage are they use cross-vaildtion data set for testing. So you can easyly find which algorithm is best fit to your dataset by their accouracy level. 



Reference :

Getting Started with Weka : https://goo.gl/EQvD8Y


