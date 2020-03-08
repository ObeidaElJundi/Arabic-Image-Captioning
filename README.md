# Arabic-Image-Captioning
Generate Arabic captions for images using Deep Learning

Paper: to be added soon.

Dataset: [./data/Flickr8k_text/Flickr8k.arabic.full.txt](./data/Flickr8k_text/Flickr8k.arabic.full.txt)

Presentation: [here](https://drive.google.com/file/d/1vt1LcE_0xEFHpQ95bLWLNWqrwZ9AbTS8/view?usp=sharing)

## Introduction
Image Captioning refers to the art of describing the content of an image by computers. It is a well-known problem in CV and NLP. It has many applications, such as improved information retrieval, early childhood education, for visually impaired persons, for social media, and so on. Although remarkable work has been accomplished recently for English, and due to the lack of large and publicly available dataset, the progress on Arabic Image Captioning is still lagging. Therefore, we developed our own dataset based on Flickr8K. It can be found under **data/Flickr8k_text/** folder, named **Flickr8k.arabic.full.txt**. It has the exact same format as the original Flickr8K.

## Model
Inspired by recent advances in neural machine translation, the sequence-to-sequence encoder-decoder approach was adopted here.
![seq2seq-image-captioning-arabic](https://user-images.githubusercontent.com/9033365/50055387-e3ab9980-0156-11e9-859f-dce71314777a.png)
For mode details, please check the paper.

## Results
Good example:
![good_examples](https://user-images.githubusercontent.com/9033365/50055400-181f5580-0157-11e9-8a00-1d7af672b49f.png)
<br /> <br />
Bad example:
![bad_examples](https://user-images.githubusercontent.com/9033365/50055408-2a998f00-0157-11e9-9d63-2b40e46a78f7.png)

Results show that developing language specific datasets and end-to-end models outperforms translating English generated captions to a destination language as the later may accumulate both models errors: image captioning and translation.

![6](https://user-images.githubusercontent.com/9033365/76162680-71f3ad00-6159-11ea-9b19-e8957435336b.PNG)

## Installation
1. Clone or download this repository.

2. Make sure python 3.x is installed on your PC. To check if and which version is installed, run the following command:
```
python -V
```
If this results an error, this means that python isn’t installed on your PC! please download and install it from [the original website](https://www.python.org/)

3. (optional) it is recommended that you create a python virtual environment and install the necessary libraries in it to prevent versions collisions:
```
python -m venv AIC
```
where AIC is the environment name. Once you’ve created a virtual environment, you may activate it.
```
AIC\Scripts\activate.bat
```

4. Install required libraries from the provided file (**requirements.txt**):
```
pip install -r requirements.txt
```
Make sure you provide the correct path of **requirements.txt**

5. Open jupyter notebook:
```
AIC\Scripts\jupyter-notebook.exe
```
then navigate to and open [Arabic Image Captioning.ipynb](./Arabic%20Image%20Captioning.ipynb)


## Citation
To be added soon.

## Contact information
For help, issues, or personal communication related to this work, please contact Obeida ElJundi: [oae15@mail.aub.edu](mailto:oae15@mail.aub.edu)
