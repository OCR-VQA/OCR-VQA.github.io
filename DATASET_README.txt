The KVQA Dataset can be divided into three parts:

1. KVQA1.0 - dataset images - http://dosa.cds.iisc.ac.in/kvqa/KVQA_images.tar.gz

2. KVQA1.0 - reference images - http://dosa.cds.iisc.ac.in/kvqa_reference_images.tar.gz

3. KVQA1.0 - Other supporting files - http://dosa.cds.iisc.ac.in/kvqa/KVQA_json.tar.gz

-----------------------------------------------------------------------------------------

1. KVQA1.0 - dataset images: It contains a folder named KVQA_images which contains 24,602 images containing 1-face, 2-face, 3-face, 4-face and 5-face images. 

2. KVQA1.0 - reference images: It contains a folder named KVQA_reference_images which contains 69,409 images. 

3. KVQA1.0 - Other supporting files: This contains a json file named dataset.json. It contains
dataset.json which contains data in the following json format
{
	ImgId:{
		'NamedEntities': A list of named entities present in the image, 
		'Qids': Corresponding of Qids,
		'wikiCap': Wiki Caption associated with the image,
		'Questions': A list of questions associated with the image,
		'Answers': A list of answers to the questions,
		'ParaQuestions': Paraphrase version of the questions,
		'Type of Question': A list of tags like Boolean, Spatial, etc for each question,
		'sourcePath': URL from where the image has been downloaded
	}
}

------------------------------------------------------------------------------------------


