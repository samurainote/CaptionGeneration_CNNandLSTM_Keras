# CNN and RNN: Image Caption Generation
## VGG16とGloveで転移学習を行なった画像キャプション生成
![](https://zhenguochen.github.io/content/images/2017/05/Untitled-Diagram.png)

## Introduction

CNN-LSTM model:

The caption generation model is roughly divided into three networks.

1. CNN layer: convert image to vector (For CNN, I used existing models for image classification VGG_ILSVRC_19_layers.)
2. Word embedding layer: word to vector conversion by using Glove
3. LSTM layer: Input vector and output probability of next word

I used pre-trained weights from Glove for word2vec and VGG16 for feature extraction from Image.

## Technical Preferences

| Title | Detail |
|:-----------:|:------------------------------------------------|
| Environment | MacOS Mojave 10.14.3 |
| Language | Python |
| Library | Kras, scikit-learn, Numpy, matplotlib, Pandas, Seaborn |
| Dataset | [Flicker8k](https://forms.illinois.edu/sec/1713398) |
| Algorithm |  CNN-LSTM Network |

## Refference

- [Develop an image captioning deep learning model using Flickr 8K data](https://fairyonice.github.io/Develop_an_image_captioning_deep_learning_model_using_Flickr_8K_data.html)
- [Image Captioning with Keras](https://towardsdatascience.com/image-captioning-with-keras-teaching-computers-to-describe-pictures-c88a46a311b8)
- [Multi-Modal Methods: Image Captioning (From Translation to Attention)](https://medium.com/mlreview/multi-modal-methods-image-captioning-from-translation-to-attention-895b6444256e)
- [Image Captioning Using Neural Network (CNN & LSTM)](https://zhenguochen.github.io/image-captioning-using-neural-network-cnn-lstm/index.html)
- [How to Prepare a Photo Caption Dataset for Training a Deep Learning Model](https://machinelearningmastery.com/prepare-photo-caption-dataset-training-deep-learning-model/)
- [How to Use Small Experiments to Develop a Caption Generation Model in Keras](https://machinelearningmastery.com/develop-a-caption-generation-model-in-keras/)
- [anuragmishracse/caption_generator on GitHub](https://github.com/anuragmishracse/caption_generator/blob/master/caption_generator/prepare_dataset.py)
- [Chainerで画像のキャプション生成](https://qiita.com/dsanno/items/b237482087207d0364c3)
