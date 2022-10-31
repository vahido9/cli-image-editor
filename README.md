# Command Line Image Editor
## About the Project
This application allows you to apply up to 9 filters to your image of choice. Each filter modifies the inputted image's pixels and then returns a copy of the filtered image which you can save. This project was developed by me, Vahid in 2019.

## Getting Started
### Prerequisites 
- Python3 or later
- pip 20.0.2 or later
	- Unix installation:
		```powershell 
		python -m ensurepip --upgrade
		```	
	- Windows installation: 
		```powershell
		C:> py -m ensurepip --upgrade
		```
- Pillow 
	```powershell
	python3 -m pip install --upgrade pip
	python3 -m pip install --upgrade Pillow
	```
### Installation
1. Clone the repo.
```
git clone https://github.com/vahido9/cli-image-editor.git
```
2. Add any desired pictures you wish to edit in the `/images` directory. 
### Usage
The **cli-image-editor** can be run in one of two ways.
1. Execute `__main__.py`
```powershell
python3 __main__.py
```
- You will be shown a prompt of all the program's commands: 
	```
	L)oad image S)ave-as
	2)-tone    3)-tone   X)treme contrast   T)int sepia   P)osterize
	E)dge detect    I)mproved edge detect   V)ertical flip   H)orizontal flip
	Q)uit
	```
- Begin by loading an image with its file extension into the program by entering the **L**oad command.
	```powershell
	$ : L
	$ Enter the name of an image file: dog1.jpg
	```
- If the image exists, it will be previewed to you. ![Image](https://github.com/vahido9/cli-image-editor/blob/main/images/dog1.jpg "Loaded Image"). **Close the preview to continue**
- Apply the desired filter on your image: 
	```powershell
	$ : X
	```
- The filtered image popups. ![Filtered Image](https://github.com/vahido9/cli-image-editor/images/extremeContrastDog1.jpg "Filtered Image")
- You can continue applying more filters or save your filtered image in your destination of choice.
- - - - - 
2. Using the batch script
```
python3 run_batch.py
```
- The batch script can be found under **/batch/batch_script.txt** and is modifiable.
- The syntax of the script is shown in the following table and example: 

Image name | Name to Save Image As | Filter code(s)
-----------|-----------------------|--------------
dog1.jpg   | dog1WithFilters       | X T 3 E

- Filter codes are as follows: **2**-tone, **3**-tone, **X**treme contrast, **T**int sepia, **P**osterize, **E**dge detect, **I**mproved edge detect, **V**ertical flip, **H**orizontal flip.