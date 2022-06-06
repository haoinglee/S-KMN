## 1. Summary
This dataset is a real-world dataset of junior high school physics quiz questions, with a total of 19,410 questions, covering 30 knowledge units from grade 7th to 8th. It is provided by our collaborator, an educational technology company. 
Some sample questions are publicly available at https://github.com/haoinglee/S-KMN.
The sample datasets publication and full datasets usage for academic research is permitted, after the consensus is reached, all datasets will be publicly available.
_The process of labeling dataset:_ 
The dataset is manually labeled by a team of professional teachers in our collaborating company. To ensure labeling quality and consistency, three annotators, with specialized knowledge of physical disciplines, participated in the annotation task. The entire annotation proceeds in a two-stage process, where the annotators independently label the entire dataset of 19,410 questions in stage 1, and each of the questions where the annotators do not have complete agreement is negotiated by all annotators to determine the final knowledge unit in stage 2. This process produces high-quality knowledge units for the physics quiz question dataset. This dataset was generated on April 26, 2020.
_Dataset Overview:_

- Each question consists of the question text and the option, annotated knowledge units and question types.
- The data are contained in the files train.csv, test.csv, ratings.csv and tags.csv. More details about the contents and use of all these files follows.

## 2. Usage License
Neither the Central China Normal University nor any of the researchers involved can guarantee the correctness of the data, its suitability for any particular purpose, or the validity of results based on the use of the data set. The data set may be used for any research purposes under the following conditions:

- The user may not state or imply any endorsement from the Central China Normal University or the National Engineering Research Center for E-Learning (NERCEL).
- The user must acknowledge the use of the data set in publications resulting from the use of the data set (see below for citation information).
- The user may redistribute the data set, including transformations, so long as it is distributed under these same license conditions.
- The user may not use this information for any commercial or revenue-bearing purposes without first obtaining permission from a faculty member of the NERCEL at the  Central China Normal University.

*The executable software scripts are provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of them is with you. Should the program prove defective, you assume the cost of all necessary servicing, repair or correction.
In no event shall the Central China Normal University, its affiliates or employees be liable to you for any damages arising out of the use or inability to use these programs (including but not limited to loss of data or data being rendered inaccurate).

If you have any further questions or comments, please email _lihao205@mail.ccnu.edu.cn_
## 3. Further Information About our research team
Our research team is affiliated with the National Engineering Research Center for E-Learning at the Central China Normal University. Our research projects have explored a variety of fields including:

- Intelligent educational application
- classroom learning behavior analysis
- multimodal learning 
- organization and management of educational resources
- subject knowledge representation.

If you have exciting ideas for experimental work to conduct on our physics quiz question dataset, send us an email at _lihao205@mail.ccnu.edu.cn_ , we are always interested in working with external collaborators.
## 4. Content and Use of Files
During the pre-processing step, the Chinese word segmentation tool PkuSeg, based on the physics dictionary, is applied to the question text. Based on word segmentation, useless information such as stop words, punctuation, and number are removed from the tokenized sequence data.
### 4.1 Samples.csv
The data in this file are some sample questions from the dataset.  Each line of this file after the header row represents one question and has the following format:
_question_id , type_id , titles , options , knowledge_id_
These questions may have errors and inconsistencies due to manual entry or direct crawling of the question text by the website.
### 4.2 question types.csv
（1）All question types are contained in the file _**question**_ _**types.csv**_. Each line of this file after the header row represents a question type and its serial number, in the following format:
_type_id , question_type_

（2）The dataset contains six question types, such as multiple choice questions, calculation questions, fill-in-the-blank questions, and experimental questions, etc. The question types and the corresponding quantity distribution are shown in the following figure, among which multiple choice questions and fill-in-the-blank questions account for a large proportion.
![fig5-eps-converted-to_00.png](https://cdn.nlark.com/yuque/0/2022/png/2000063/1653883226009-25bd2ecd-f091-468f-95ab-dcdd1ddf1568.png#clientId=u4ab5c72c-b4b5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=455&id=ucddc8e6b&margin=%5Bobject%20Object%5D&name=fig5-eps-converted-to_00.png&originHeight=1819&originWidth=2011&originalType=binary&ratio=1&rotation=0&showTitle=false&size=164421&status=done&style=none&taskId=u5ebd93e9-aa62-4f31-8a78-8a8f245452c&title=&width=503)
### 4.3 knowledge units.csv
All knowledge units are contained in the file _**knowledge**_ _**units.csv**_. Each line of this file after the header row represents a knowledge unit and its serial number, in the following format:
_knowledge_id , knowledge_unit_




