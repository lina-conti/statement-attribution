# :newspaper: Statement attribution
Final project for NLP in Industry course 2022

## Presentation

This is an M2 university project by [Lina Conti](https://github.com/lina-conti) and [Isaac Murphy](https://github.com/isaac-murphy) for the NLP in Industry course.

We developped a system that identifies the person who is expressing an opinion in a newspaper article paragraph. 

We were given a corpus and shared the annotation task among all members of the class. We were given full freedom as to what type of model to implement to solve the task at hand. Our group implemented three different neural networks:

- a [bilinear LSTM mono-label classifier](https://github.com/lina-conti/statement-attribution/blob/main/Monolabel_Classifier_Industry_Conti_Murphy.ipynb) that predicts one speaker from a list of all speakers present in the training corpus
- a [bilinear LSTM sequential classifier](https://github.com/lina-conti/statement-attribution/blob/main/Vanilla_Sequential_Classifier_Industry_Conti_Murphy.ipynb) that predicts for each token if it is inside (I), outside (O) or at the beginning (B) of the name of a speaker (so only speakers explicitly mentioned are recognized)
- a [bilinear LSTM sequential classifier pre-trained on the named entity recognition task](https://github.com/lina-conti/statement-attribution/blob/main/Transfer_learning_sequential_classifier_industry_Conti_Murphy.ipynb), which is the best performing system among the three.

Our final report can be found [here](https://raw.githubusercontent.com/lina-conti/statement-attribution/main/Conti_Murphy_NLP_in_Industry.pdf).
