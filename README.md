# Art-CNN


## Identifying Art styles with Convnet
This notebook runs on a part of the https://www.kaggle.com/c/painter-by-numbers dataset containing only 4 of the Art styles (Abstract Expressionism, Cubism, Early Renaissance, Ukiyo-e). I shared the dataset as well for those interested in running the same analysis.

I wanted to create a Convnet that was indentifying art styles. There is many art style in the original dataset, some with more than 8000 images in them. For RAM/time analysis reasons I used art that were:

very different (Cubism/Renaissance) instead of going with very similar art styles (Early VS late renaissance);
I also chose those because they had enough data to create an accurate CNN but not so many that the analysis were taking too long (around ~1000 images each in the train set).
I took the VGG16 pretrained model to identify the images and add a few layers of hidden neurons.

I also display 10 random images taken of the testset and plot them with they prediction and proability after.
