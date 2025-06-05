Medicinal vs Non-Medicinal Classification
1.	Used a combination of images to prepare dataset for medicinal and non_medicinal plants
2.	Datasets used: 
a.	https://www.kaggle.com/datasets/kacpergregorowicz/house-plant-species
b.	https://www.kaggle.com/datasets/sanjanatelang/medicinal-plants-roots-dataset
c.	Few images from https://www.kaggle.com/datasets/noahbadoa/plantnet-300k-images
3.	Pre trained Model used: EfficientNetB0
4.	Advantages of EfficientNetB0
a.	Excellent Accuracy-to-Size Ratio: achieves strong classification performance on benchmarks like ImageNet, comparable to deeper models like ResNet50 or VGG16, but with far fewer parameters.
b.	Fewer Parameters & FLOPs: ~5.3 million parameters
c.	Compound Scaling: EfficientNet uses a compound scaling method to scale depth, width, and resolution in a balanced way.
d.	Faster Inference Time: Due to its lightweight nature, inference is faster compared to heavier architectures like ResNet or DenseNet, especially on CPU and mobile devices.
e.	Transfer Learning Friendly: Pretrained weights are readily available.
f.	Better Regularization and Training Stability: Uses Swish activation and squeeze-and-excitation (SE) blocks, which help improve feature extraction and training stability.
5.	Input image size: 224, 224
6.	Train-test split: 70 and 30%
7.	Images distribution: 
a.	Medicinal: Around 15k
b.	Non-Medicinal: Around 12k
8.	Accuracy achieved: 
a.	Training: ~98%
b.	Validation: ~75%


Plant Leaf Image Classification
1.	Datasets used: 
a.	https://www.kaggle.com/datasets/ichhadhari/leaf-images
b.	https://www.kaggle.com/datasets/meetnagadia/collection-of-different-category-of-leaf-images
2.	Filtered only the medicinal plant leaves from this dataset
3.	Classes used to train the model: 
a.	'Alstonia Scholaris (P2)',
b.	 'Apta',
c.	 'Arjun (P1)',
d.	 'Basil (P8)',
e.	 'Chinar (P11)',
f.	 'Gauva (P3)',
g.	 'Jamun (P5)',
h.	 'Jatropha (P6)',
i.	 'Karanj',
j.	 'Kashid',
k.	 'Lemon (P10)',
l.	 'Nilgiri',
m.	 'Pimpal',
n.	 'Pomegranate (P9)',
o.	 'Sita Ashok',
p.	 'Sonmohar',
q.	 'Vad',
r.	 'Vilayati Chinch']
4.	Pretrained model used: Xception
5.	Advantages of Xception:
a.	Depthwise Separable Convolutions (Efficiency + Power): The core innovation is the use of depthwise separable convolutions, which break standard convolution into:
i.	Depthwise convolution (one filter per channel)
ii.	Pointwise convolution (1×1 convolution to mix channels)
b.	High Accuracy: Delivers comparable or better performance than many traditional CNNs like ResNet or VGG, especially with fewer parameters than similarly-performing models.
c.	Good for Transfer Learning: Widely used as a backbone for transfer learning, especially in image classification, object detection, and segmentation.
d.	End-to-End Architecture: Unlike Inception modules that require manual optimization of layer types (1×1, 3×3, etc.), Xception uses a uniform architecture with depthwise separable convolutions, making it easier to implement and tune.
e.	Better Parameter Utilization: Achieves higher accuracy per parameter, meaning it uses its computational budget more effectively than traditional convolutions.
6.	Dataset size: 4352, Classes: 18
7.	Train-Val split: 80% and 20%
8.	Accuracy achieved: 
a.	Train accuracy: 0.9841
b.	Validation accuracy: 0.9688
