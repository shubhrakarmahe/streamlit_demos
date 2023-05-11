<b>Neural style transfer</b> is an optimization technique used to take two images—a content image and a style reference image (such as an artwork by a famous painter)—and 
blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.
This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image.
These statistics are extracted from the images using a convolutional network.

NST was originally published in a 2015 article by Leon Gatys. The original article used VGG19 (a convolutional network trained on Imagenet) as a model.
Later, Google released a method that allowed several styles to be applied at the same time. Since then, a lot of templates and apps have come out.

we will use Sreamlit, a Python library that allows us to create web apps. Not only that, but it also allows us to be able to deploy to the cloud (you just need to have an account on GitHub).

Step 1: create app.py file in which we first insert the libraries we need.

Step 2: create functions that allow us to load images into our app.

Step 3: preprocess the images i.e. rescale the image and transform it into a tensor.

Step 4: transform the output tensor to an image.

Step 5: load pre-trained model (https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2) from TensorFlow Hub

Step 6: write a function that combines all the above elements together.

Step 7: post-process the resulting image

Step 8: create streamlit web app

Step 9: deploy the app to streamlit cloud by using Github code repo


App link: https://shubhrakarmahe-streamlit-demos-neural-style-transfarapp-fwjcdl.streamlit.app/

Reference Links:-
1. https://www.tensorflow.org/tutorials/generative/style_transfer
