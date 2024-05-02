## Project: Empathy Classification in Text-Based Online Mental Health Support

This is the final project for Natural Language Processing with Deep Learning @ MIDS. Our team includes Nicole Liu and Ambika Gupta.

### Introduction

While mental health issues are on the rise, professional support is struggling to fulfill the demand. In this context, many individuals still default to online forum such as Reddit to share their experiences, ask for advice, and seek help. The range of responses they may receive for a particular post is broad, arbitrary, and unregulated. Some responses show empathy and provide practical advice, while others are unhelpful or even exacerbate the problem by assigning blame.

As these forums have been operating for several years, there is now a vast amount of text-based pairs of posts seeking help and posts responding to them. In this paper, we adopt the framework developed by Sharma et al (2020) to evaluate responses for empathy. EPITOME measures three communication mechanisms of empathy: emotional reaction, exploration, and interpretation. This framework combines the emotional and cognitive components related to the exchange of experiences, feelings, and understanding.

In our work, we use three sub-datasets, each corresponding to one of the three aspects of empathy. Our tasks were binary classifications of whether the responses showed emotional reaction, exploration, or interpretation, respectively for each dataset.

Our major contributions are twofold.

(1) While the original paper by Sharma et al applies a uniform approach of feature engineering in all three datasets, we instead propose distinct feature engineering techniques depending on the aspect of interest.

(2) Recognizing the challenge of data collection and annotation in the real world, our work utilized a substantially smaller dataset, less than 30% of the original data used by Sharma et al.

With this work, we hope to evaluate the presence of empathy in text-based mental health support in a more efficient way and guide the effort of generating more relevant and impactful mental health resources on a large scale.

### Conclusion

In this project, we used the data with annotated empathy levels from the EPITOME framework and performed binary classification tasks on the Emotional Reactions, Interpretations, and Explorations datasets. We augmented data with back-translation, experimented with various feature engineering techniques to improve BERT-based models, and tested our highest performing features on BERT variants. Our best models achieved accuracy scores of 81% - 93% and F1 scores of 81% - 92% across the three datasets. Notably, we found that different feature engineering techniques worked best for different datasets. The Explorations dataset had the best results among the three datasets, especially with ALBERT.

Future work includes multiclass classification using the original three labels in the data to further detect nuances in empathy levels. Additionally, mention detection techniques applied to rationale extraction would also complement the classification task.
