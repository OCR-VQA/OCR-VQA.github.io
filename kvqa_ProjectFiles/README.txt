OCR-VQA dataset contains 207572 images and associated question-answer pairs.
The images of this dataset are obtained from following paper:

Brian Kenji Iwana, Seiichi Uchida:
Judging a Book By its Cover. CoRR abs/1610.09204 (2016)

We provide questions inquiring about title, author, edition, year and
genre of the book and corresponding ground-truth answer. This dataset
contains approximately 1 million QA pairs.


Getting started
---------------------------------------------------------------
Download instructions:
---------------------
Download following zipped folder containing a json file
and data loader python script:

LINK HERE

Getting info about dataset:
---------------------------
OCR-VQA dataset can be loaded using the script downloaded above as follows:

>> python loadDataset.py

dataset contains alphanumeric characters of length 9 as keys. Each key contain
following fields

'imageURL': URL of image
'questions': a list of questions
'answers': a list of corresponding answers


Example:
-----------------------------------------------------------
Example to get different information about one image (Key: '470536764'):

dataset['470536764']['imgURL']
http://ecx.images-amazon.com/images/I/51wjgMtqUSL.jpg

dataset['470536764']['questions'][0] # First question for this image
'Who wrote this book?'

dataset['470536764']['answers'][0] # Ground-truth answer of first question
'Robert Biswas-Diener'

dataset['470536764']['questions'][3] # Fourth question for this image
'Is this book related to Science & Maths?'

dataset['470536764']['answers'][3] # Ground-truth answer of fourth question
Yes

------------------------------------------------------------------
If you use this dataset, please cite our ICDAR 2019 paper.

@InProceedings{mishraICDAR19,
  author    = "Anand Mishra and Shashank Shekhar and Ajeet Kumar Singh and Anirban Chakraborty",
  title     = "OCR-VQA: Visual Question Answering by Reading Text in Images",
  booktitle = "ICDAR",
  year      = "2019",
}
-----------------------------------------------------------------

For any queries about the dataset feel free to contact: anandmishra@iisc.ac.in.
