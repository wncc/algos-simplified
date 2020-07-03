# Object Detection Algorithms

Have you ever wondered how an automonous car detects other cars on the road, the traffic lights and pedestrians? Have you ever given a thought how does security surveillance systems work?  

These systems are powered by the Object Detection Algorithms. We discuss about the prominent ones this week. 

* To get an overview of the Object Detection field, head **[here](https://towardsdatascience.com/how-does-ai-detect-objects-technical-d8d63fc12881)**.  

We start with the family of RCNN's and then proceed to SSD, YOLO which are more advanced algorithms for Object Detection.  

## Region Based Convolutional Neural Networks (RCNN's)

Before deving into the algorithm brush up your understanding of **[CNN](https://medium.com/jun-devpblog/dl-8-cnn-1-convolutional-neural-network-basics-2f60c93d7d22)**.  

As a pre-cursor, we could have used CNN's directly for object detection using the following approach - 
* We split up the image into various parts.
* The setions are then fed into a CNN and classified on some pre-defined classes. 
* Then the entire image is combined to spot the objects in the image.

But this has a lot of issues - 
* One object can span multiple sections of image and hence hars to classify.
* We might need very small sections so that the smaller objects can be identified that makes in computationally inefficient. 

So, to overcome this, the Region based CNN was introduced.  

The steps that we follow are - 
* The image is taken as input and the Regions of Interest are identified based on selective search. 
* These regions are then rescaled to match the pre-trained CNN input shape and passed through the network to extract features. 
* These are then fed to SVM's to classify it into different classes. 
* A bounding box regression is then performed in order to fit the object as perfectly as possible.  

For a detailed explanation, refer to this **[video](https://www.youtube.com/watch?v=uX4LLf-33p0)**. 

The computational expense of RCNN's owing to the complexity of the architecture that includes CNN's, SVM's and Regressors makes it practically infeasible for large datasets. To overcome this challenge, Fast RCNN's were introduced, which we discuss in the next section. 

## Fast RCNN's

Basically we get rid of Explicit Selective Search before CNN, SVM's after the CNN and the linear regressor in the end to make it faster and more efficient. Obtaining Regions of Interest, extracting features, classification and regression all these steps are now performed by the CNN itself.  

* Regions of Interest are made to be output by the Conv Net.  
* The regions are then reshaped to the desired input shape using a Pooling Layer. 
* Then a softmax layer does the job of classification. 
* A linear regression layer in the end does the bounding box regression.  

To dive deeper into the algorithm, go through this **[video](https://www.youtube.com/watch?v=xzw3lcdllOU)**. 

Though the Fast RCNN is much faster than the RCNN, another improvement called the Faster RCNN is much faster than the two algorithms we discussed. 

## Faster RCNN's 

In Fast RCNN, we got rid of the explicit Selective Search, but it is still being performed by the CNN to obtain the Regions of Interest, so in this improvement, we get rid of it completely and bring in a new architecture calles the Region Proposal Network.  

The only difference is in the first two steps - 
* The entire image is fed to the CNN to obtain feature maps. 
* The Region Proposal Network is applied on these feature maps and Objectness Score is obtained for various object proposals.  

To go deeper into the three algorithms that we discussed, refer to these linkes - 

* **[Video](https://www.youtube.com/watch?v=v5bFVbQvFRk)** 
* **[RCNN](https://towardsdatascience.com/r-cnn-3a9beddfd55a)**
* **[Comparison of various RCNN Algorithms](https://www.geeksforgeeks.org/r-cnn-vs-fast-r-cnn-vs-faster-r-cnn-ml/)**

We now discuss a relatively advanced algorithm called SSD. 

## Single Shot Multi-Box Detector (SSD)

This algorithm is a great improvement over traditional RCNN algorithms in the field of object detection. 

The three terms in the name of the algorithm give a high level introduction to what the algorihtm is - 

* **Single Shot** - It means that object localisation and object classification is done in a single forward pass of the network.
* **Multi-Box** - It refers to the Bounding Box Regression employed in such a network. 
* **Detector** - The network that is used in the architecture also classifies the object that is detected by it.  

#### Useful Resources

* For a complete information on SSD, head **[here](https://towardsdatascience.com/understanding-ssd-multibox-real-time-object-detection-in-deep-learning-495ef744fab)**. 
* Refer to **[this](https://www.youtube.com/watch?v=5rY7CevPkKM)** video for an in depth explanation on this algorithm.  

There are a few challenges faced by this Algorithm. Let us first get through these challenges and then we proceed to the YOLO Algorithm. 

* Small objects are hard to detect because of the fact they may not appear in all feature maps.
* A large amount of time is spent on the CNN used (VGG-16), that means that one can make SSD faster by a great factor if we can come up with a more efficient and simpler architecture. 

## You Only Look Once (YOLO)

This has revolutionised the Object Detection Domain but pretty accurate and time efficient results. 

In the traditional methods, we detect objects using the Region Proposal Network that makes it computationally redundant as prediction step is performed on some regions multiple times that can be avoided. This done by invoking a CNN i.e. a Fully Convolutional Network rather than a Region Convolutional Network. Baiscally, the image is fed into the the network and a grid like structure is the output along with bounding box and class probabilites associated with it. 

For detailed explanation, refer to this **[video](https://www.youtube.com/watch?v=9s_FpMpdYW8)**.  

Let us look at a few advantages of this algorithm over the other algorihtms that we looked at -

* This is really fast as the pipeline is really simple which is due to the fact that frame detection is performed as a regression problem. 
* Since, it takes the entire image at once, it is able to see the context and avoid detecting patches as objects. 
* It is able to learn generalisable object representations that can be utilised in new domains and that makes it really powerful.  

This **[article](https://towardsdatascience.com/yolo-you-only-look-once-real-time-object-detection-explained-492dc9230006?gi=b3f5dce164a7)** explains the concepts in great detail. 

Next week, we will come up with new exciting algorithms, till then keep exploring the domain of Object Detection Algorithms. 
