# -Parallel-Image-Classification-using-CNN
This repository demonstrates an implementation of parallel image classification using Convolutional Neural Networks (CNNs). The project explores how CNNs can be structured to process image data in parallel, enhancing computational efficiency and enabling experimentation with various filter sizes and layer configurations for improved accuracy.

Keywords:
CNN, parallel programming, image classification, CUDA, Deep learning

List of references:
https://www.linkedin.com/pulse/forward-back-propagation-over-cnn-code-from-scratch-coy-ulloa/ https://www.jefkine.com/general/2016/09/05/backpropagation-in-convolutional-neural-networks/ https://arxiv.org/pdf/1511.08458.pdf https://jmyao17.github.io/Machine_Learning/Neural_Network/CNN-1/CNN_Build.html

1. Summary:

Due to this your group will make a song which will be used to divide the class image using the network Convolution Neural Network (CNN). My CNN consists of multiple layers combined together: It will be increased faster with your weekly version. The application will be executed on NVIDIA CUDA GPU.

2. Background

In recent years, there has been considerable research development on the use of CNN for tasks related to image recognition and classification. The basic idea of ​​our CNN model is to take an image as input and extract more complex features at each layer with lower resolution. Out of these layers, some layers are activated to make decisions and predictions about the image.

To create a CNN model, a large amount of data is needed to get a very small set of them. That is, this makes mining very heavy on calculations and can take many hours, even days, to run on a traditional CPU.

During this project, the group wanted to exploit the features of each class of CNN such as Pooling, FullyConnected, Convolution,... and modified the transmission algorithm to fit the CUDA architecture and achieve higher speed.

3. The challenge

The process of generating a network in a short time (CNN) is a task that requires specialized depth of calculation, so it requires the ability to perform a single song to reduce the time taken. The content that is being trained is becoming more and more important every day, and the work that is being done to create CNN network is becoming more important. What problems have to be faced when the song is sung.

* The calculation result of each class needs to be shared among all the threads because the calculation of the next class depends on the result of the previous class. Therefore, CNN's communication ratio to calculate is very high, leading to high performance on GPU.
* Limited memory: The amount of memory generated for computing songs is significantly limited because the memory is limited to the GPU.
* The classes that belong to each other should not only sing within a class, not between classes. To overcome these challenges, the group optimizes the CNN architecture to use less memory and has less demand. Better communication, reuses memory so that it does not have to be loaded multiple times from CPU to GPU.

4. Resources

For this group, I use a Colab computer (Tene CPU: Persistence M, 13GB Ram, Tene GPU: Tesla T4) to proceed and set a weekly program and a song to train my CNN. The source setting for this CNN will be built from scratch, which can be used to support some libraries such as Numpy. Here's what I read on CNN: https://arxiv.org/pdf/1511.08458.pdf. The raw materials for training data are available in tensorflow libraries such as MNIST, CIFAR-10,...

5. Goals And Deliverables
* During this period, the group will start running a song on CNN's network. The goal of the group is to build the same version of the same song with the same speed as that of the same (or slower than not too many) so with the model built from the standard libraries (keras, tensorflow, pytorch,... .) Because this is the framework that provides the best speed. Or at least the application is designed to run faster with its weekly version. If the progress of your project is faster and better, the group can use the optimized application for memory size, or make the song song as part of the data set in 3D.
* The group will demo the application using the song I am playing and compare the time it runs on different types of data. The group will also present some of the speed graphs that the group uses, as well as some of the optimization methods that the group has used.
* Questions that the team needs to answer in project analysis: What work needs to be done to carry out the project and how long will it take? How is each member's work divided? How long does it take for each job? If a member has not completed the work before the deadline, how should it be resolved? What risks may occur during project implementation? Will the project produce the desired results? Is optimizing application time necessary? What is the biggest benefit of the project?
The application can parallelize independent tasks such as convolution, matrix multiplication, batch calculations, etc. The performance of the parallel version that the team hopes to achieve can be about 10-30 times faster. times compared to sequential installation.
