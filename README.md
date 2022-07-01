# ResNet50
Transfer Learning With Keras(Resnet-50)
So, What is Transfer Learning?
Simply put, transfer learning is the phenomenon which allows you to transfer what state-of-the-art machine learning models have learnt, and you use it for your custom problem.

The following flow chart represents how transfer learning works in practice. Deep learning model 1 transfers the knowledge it learnt(weights, biases) which can be then used by deep learning model 2.
[](https://chroniclesofai.com/content/images/2021/07/image-10.png)

Okay, but why do we need transfer learning. Why can't we train our own neural networks from scratch?

Most deep learning networks that are used for real world problems, learn around millions of parameters to give a high accuracy.

Now let's say i am working on the problem of face detection. Sure I can train my deep learning model from scratch for this.

But here's the catch:

Any image classification network will learn very similar weights and features in order to identify a face.
So why not use what state of the art models have learnt and use it for our problem?

Models that have been trained on extensive data sets like COCO or ImageNet, are in general good at recognizing objects in images. So it only makes sense to directly use what they have learnt and fine tune it to our purpose.

So in short, transfer learning allows us to reduce massive time and space complexity by using what other state-of-the-art models have learnt.
With the basics out of the way, let's start with implementing the Resnet-50 model to solve an image classification problem.
