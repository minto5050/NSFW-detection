# Tensorflow NSFW Image classifier

This is the repository developed for 'Image Classifier in TensorFlow in 5 Min on [YouTube](https://youtu.be/QfNvhPx5Px8) using this [CodeLab](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/?utm_campaign=chrome_series_machinelearning_063016&utm_source=gdev&utm_medium=yt-desc#0) by Google as a guide. 

Applications can use this model to detect nudity in the images using tensorflow.

```Final test accuracy = 98.2% (N=1098)```

training command

```python retrain.py \ --bottleneck_dir=bottlenecks \ --how_many_training_steps=500 \ --model_dir=inception \ --summaries_dir=training_summaries/basic \ --output_graph=retrained_graph.pb \ --output_labels=retrained_labels.txt \ --image_dir=trainimg```

Give a test image to verify the model

```python classify.py test_image.jpg```
