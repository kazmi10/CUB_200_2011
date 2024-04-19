# Machine-Learning-Neural-nets-Fine-grained-image-classification

# Fine-grained image classification | Using Birds Dataset| 200 categories of birds
This project uses the Caltech-UCSD Birds-200-2011 Dataset, found at:

http://www.vision.caltech.edu/visipedia/CUB-200-2011.html

# Code Description 
. The code is distributed across two .ipynb files, with detailed annotations provided to enhance comprehension.

. It is recommended to open these files in Colab for optimal viewing, as Markdown annotations are utilized extensively.

. All cell outputs are included for convenience, eliminating the need to execute the code manually. This is particularly beneficial since some models require significant computational time to complete.

# 1_Descriptive_Analysis
The initial file, labeled "1_Descriptive_Analysis," encompasses the code utilized for dataset analysis.

1. The structure of this initial file unfolds as follows:

2. Relevant packages are imported.
   
3. Descriptive analysis is performed on the dataset, with the execution time averaging approximately one hour.

# 2_Model_Implementation
The second file, labeled "2_Model_Implementation," encompasses the code responsible for preprocessing the dataset and training the models.

The structure of the second file is outlined as follows:

1. Dataset preprocessing: This segment involves dividing the dataset into training and validation sets, a process that consumes approximately 1 hour to complete. The majority of this time is allocated to the dataset splitting procedure.
2. Model implementation: This section incorporates the implementation of 7 distinct models. The runtime for each model is as follows:
   - Model 1: Approximately 1.5 hours
   - Model 2: Around 3.5 hours
   - Model 3: Roughly 7 hours
   - Model 3b: Also approximately 7 hours
   - Model 4: About 1 hour
   - Model 5: Less than 1 hour
   - Model 6: Also less than 1 hour
     Given the extensive runtime of Models 3 and 3b, the results are saved to facilitate user convenience.
     
3. Results analysis: Following model training, this phase involves analyzing the results, a process that typically takes a few minutes to complete. Additionally, concise written analysis is provided in this section, with more detailed information available in the accompanying report.

# Conclusions
The primary outcome of this project is the identification of the most suitable model for the CUB-200-2011 dataset. Overall, all models performed satisfactorily on the dataset, except for LeNet. Despite being computationally intensive, EfficientNet demonstrated the best overall performance, exhibiting high accuracies and relatively low loss values. DenseNet also showed promising performance and was among the fastest models to execute, rendering it a viable option. Given that performance takes precedence over computation time, particularly considering that most fine-grain image classification models are deployed on powerful GPUs rather than Colab, EfficientNet is selected as the optimal model for the CUB-200-2011 dataset, while DenseNet is presented as a more economical alternative with slightly lower performance.

# Suggestions for Future Work
One avenue for future research involves enhancing the quality and comprehensiveness of image databases. While current databases exist, improvements in annotation quality and category coverage could enhance the performance and generalization capabilities of deep learning models. Additionally, exploiting local part information could further improve model accuracy. Fine-grained image classification benefits from leveraging part features, though current methods often rely on manual specification, limiting generalizability. Developing more efficient part detection algorithms could address this challenge.

Weakly-supervised fine-grained image classification represents another area ripe for exploration, as it remains a relatively new research focus. Furthermore, enhancing real-world applications is a primary objective in this field. Current databases often feature prominently positioned foreground objects, but including a wider variety of image layouts could improve model generalization. For instance, datasets like CUB-200-2011 primarily consist of professionally captured bird photographs, neglecting factors like lighting, blur, occlusion, resolution, and object interference. Expanding these considerations to fine-grained video recognition could also be beneficial, given their significant impact on recognition accuracy.
