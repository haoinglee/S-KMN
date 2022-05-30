# Summary

This dataset is a real-world dataset of junior high school physics quiz questions, with a total of 19,410 questions, covering 30 knowledge units from grade 7th to 8th. 
It is provided by our collaborator, an educational technology company. The dataset is manually labeled by a team of professional teachers in our collaborating company. To ensure labeling quality and
consistency, three annotators, with specialized knowledge of physical disciplines, participated in the annotation task. The entire annotation proceeds in a two-stage process, where the annotators independently label the entire dataset
of 19,410 questions in stage 1, and each of the questions where the annotators do not have complete agreement is negotiated by all annotators to determine the final knowledge unit in stage 2. This process produces high-quality
knowledge units for the physics quiz question dataset. This dataset was generated on April 26, 2020.

Each question consists of the question text and the option, annotated knowledge units and question types.

The data are contained in the files train.csv, test.csv, ratings.csv and tags.csv. More details about the contents and use of all these files follows.

The physics quiz question dataset are publicly available for download at ..............



# Usage License

Neither the Central China Normal University nor any of the researchers involved can guarantee the correctness of the data, its suitability for any particular purpose, or the validity of results based on the use of the data set. The data set may be used for any research purposes under the following conditions:

The user may not state or imply any endorsement from the Central China Normal University or the National Engineering Research Center for E-Learning (NERCEL).
The user must acknowledge the use of the data set in publications resulting from the use of the data set (see below for citation information).
The user may redistribute the data set, including transformations, so long as it is distributed under these same license conditions.
The user may not use this information for any commercial or revenue-bearing purposes without first obtaining permission from a faculty member of the NERCEL at the  Central China Normal University.
The executable software scripts are provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of them is with you. Should the program prove defective, you assume the cost of all necessary servicing, repair or correction.
In no event shall the Central China Normal University, its affiliates or employees be liable to you for any damages arising out of the use or inability to use these programs (including but not limited to loss of data or data being rendered inaccurate).

If you have any further questions or comments, please email lihao205@mail.ccnu.edu.cn

Further Information About our research team

Our research team is affiliated with the National Engineering Research Center for E-Learning at the Central China Normal University. Our research projects have explored a variety of fields including:

Intelligent educational application
classroom learning behavior analysis
multimodal learning 
organization and management of educational resources
subject knowledge representation.

If you have exciting ideas for experimental work to conduct on our physics quiz question dataset, send us an email at lihao205@mail.ccnu.edu.cn - we are always interested in working with external collaborators.

Content and Use of Files

Question Text Preprocessing

During the pre-processing step, the Chinese word segmentation tool PkuSeg, based on the physics dictionary, is applied to the question text. Based on word segmentation, useless information such as stop words,
punctuation, and number are removed from the tokenized sequence data.

Traing.csv
The data in this file is used for model training.  Each line of this file after the header row represents one question and has the following format:

question_id , type_id , titles , options , knowledge_id

These questions may have errors and inconsistencies due to manual entry or direct crawling of the question text by the website.

Test.csv
The data in this file is used for model testing, other information is similar to the file train.csv.

question types.csv
The dataset contains six question types, such as multiple choice questions, calculation questions, fill-in-the-blank questions, and experimental questions, etc. The question types
and the corresponding quantity distribution are shown in the following figure, among which multiple choice questions and fill-in-the-blank questions account for a large proportion.

All question types are contained in the file question types.csv. Each line of this file after the header row represents a question type and its serial number, in the following format:

type_Id , question_type


knowledge units.csv
All knowledge units are contained in the file knowledge units.csv. Each line of this file after the header row represents a knowledge unit and its serial number, in the following format:

knowledge_Id , knowledge_unit
