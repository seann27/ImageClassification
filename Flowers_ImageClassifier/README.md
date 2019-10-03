# Data Source
- Uses the "flowers" dataset from torchvision
	- more information can be found here -> http://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html

# Files
- train.py
	--save_dir
		- Directory where model checkpoint is saved
	--filename
		- Name of checkpoint file
	--arch
	  - Model to be used from torchvision (see pretrained_models.py for complete list)
	--learning_rate
		- Learning rate for training classifier
	--hidden_units
		- Hidden units used for training classifier
	--epochs
		- Number of training iterations

- python predict.py
	--image
		- Filepath of image
	--topk
		- Number of top predictions to display
	--json
		- File to map classes to labels

# Usage
- Run train.py, ensure you have enough space for a checkpoint file
	 -> checkpoint files can be multiple GBs if too many hidden units are used
- Run predict.py with the image you want to classify as an argument
