Lecture material
================
## 2023-03-02 [lecture 9](https://github.com/crsl4/phylogenetics-class/blob/master/lecture-notes/lecture9.pdf)
Probability model P(x) <br>
Assumptions: <br>
1.symmertic around the mean? <br>
2.Not synmmertic aorund the mean? <br>
3.How variable? concentrated around the mean or not <br>
Using possion model, only have one parameter (lambda) <br>
<img width="544" alt="Screen Shot 2023-03-02 at 1 14 09 PM" src="https://user-images.githubusercontent.com/97980830/222528766-219e7651-f7d5-4124-89a4-e5eb955c8f0b.png"> The accuracy of probability is mainly depends on the function we assumned, and the input parameter. <br>
even if it is a good model, it will never be perfect. only one paratmenter controls mean and shape of distribution. <br>

> "All models are wrong but some models are useful." --- George Box <br> 



It will depend on the assumptions of the model and the quality of input data. <br>
We need a probability model for the evolution of sequences along a phylogentic tree. --- we only focus mutation process between two seqeunces <br>
1. we need to assume the mutation process is same at every branch of tree  --- we only focus mutation process between two seqeunces <br>
2. we assume all the sites evolve independently ---- we can focus on the mutation process between two sites  <br>
3. all sites evolve the same -- we can choose any site to model the mutation process <br>
Even if we are seeing A - A, doesn't means there is no mutation at the beginning.number of mutations on time t is assumed to folow a possion distribution <br>

Jukes Cantor(JC69) assume AGCT have the same frequency <br>
Felsenstein model(F81) more realistic model becuase not setting AGCT in same frequency, based on observed sequence <br>
General Time Reversible (GTR) used a lot by recent people, it is flexible. <br>
We will cover model selection in the future class. we will to choose the model best fit for our data. it is not necessary to use complicated model. simplest model will be the best 

## 2023-03-09
## Maximum likelihood
building phylogenetic inference
step 1: choose the criterion to use distances, parsimony,llikelihood <br>
step 2: search the space of trees until you find the optimum. <br>
1.choose a substitution model <br>
2.for a given tree,calucalte the likelihood give the data and the subtituide model <br>
3.sear the space of trees using the tree moves until you find the maximum likelihood tree. <br>
calculate the likelihood for this tree dependes on parameters. Q matrix
