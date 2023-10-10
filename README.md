# Model-Library-Project

## Overview

...

## Research

### 3D model retrieval scheme

- feature tag (text)
- feature point cloud

||   |
|---|---|
|Text-based Search| Users can search for 3D models using keywords or descriptive text, similar to traditional text search engines.  |
|2D Image Retrieval|Users can provide a 2D image as a query, and the system will return 3D models that are visually similar. This method often involves computer vision techniques such as image feature extraction and matching algorithms.|



三维模型检索是指通过不同的方式来查找和获取三维模型数据的过程，通常用于计算机图形学、计算机辅助设计、虚拟现实和三维打印等领域。以下是一些常见的三维模型检索方式：

1. 文本搜索：用户可以使用关键词或描述性文本来搜索三维模型数据库。这是最常见的检索方式之一，类似于传统的文本搜索引擎。

2. 二维图像检索：用户可以提供一张二维图像作为查询，系统会返回与该图像相似的三维模型。这种方法通常使用计算机视觉技术，如图像特征提取和匹配算法。

3. 三维模型形状匹配：用户可以提供一个已知形状的三维模型，系统会搜索数据库中与之相似的模型。这通常涉及到形状描述符和匹配算法，如3D形状描述符或深度学习模型。

4. 语义检索：这种方式基于三维模型的语义信息，允许用户使用语义标签、分类或属性来搜索模型。这需要对模型进行语义注释或使用深度学习模型进行自动标注。

5. 基于内容的检索：这种方式使用模型的内部特征或属性进行检索，而不依赖于外部文本或图像查询。常见的方法包括基于形状描述符、颜色、纹理、体素网格等的检索。

6. 基于用户反馈的检索：用户可以通过与系统交互来改进检索结果。例如，用户可以选择一个模型并要求系统提供相似或相反的模型，以逐步细化搜索结果。

7. 3D模型检索引擎：一些专门的软件和搜索引擎针对三维模型检索进行了优化，提供高效的检索功能，并允许用户使用多种方式来搜索和筛选模型。

8. 基于深度学习的检索：近年来，深度学习技术已经在三维模型检索中取得了显著的进展。神经网络模型可以学习从模型数据中提取有用的特征，从而提高检索效果。

这些方式可以单独或结合使用，具体取决于应用的需求和可用的数据。三维模型检索是一个广泛研究的领域，不断涌现出新的方法和技术来提高检索的准确性和效率。

Here are some ways to perform three-dimensional (3D) model retrieval:

1. Text-based Search: Users can search for 3D models using keywords or descriptive text, similar to traditional text search engines.

2. 2D Image Retrieval: Users can provide a 2D image as a query, and the system will return 3D models that are visually similar. This method often involves computer vision techniques such as image feature extraction and matching algorithms.

3. 3D Shape Matching: Users can provide a known 3D shape as a query, and the system will search for similar models in the database. This typically involves shape descriptors and matching algorithms, such as 3D shape descriptors or deep learning models.

4. Semantic Search: This approach relies on semantic information about 3D models, allowing users to search using semantic labels, categories, or attributes. This requires annotating models with semantic labels or using automated annotation through deep learning models.

5. Content-based Retrieval: Content-based retrieval uses internal features or properties of models for searching, without relying on external text or image queries. Common methods include retrieval based on shape descriptors, color, texture, voxel grids, and more.

6. User-feedback-based Retrieval: Users can refine search results by interacting with the system. For example, users can select a model and request the system to provide similar or dissimilar models, gradually refining the search results.

7. 3D Model Retrieval Engines: Specialized software and search engines are designed for efficient 3D model retrieval, allowing users to search and filter models using various criteria.

8. Deep Learning-based Retrieval: In recent years, deep learning techniques have made significant advancements in 3D model retrieval. Neural network models can learn to extract useful features from model data, improving retrieval performance.

These methods can be used individually or in combination, depending on the application's requirements and available data. 3D model retrieval is a continuously evolving field, with new methods and technologies emerging to enhance the accuracy and efficiency of retrieval.


### Engine

- Web(html+css+javascript)+Web3D(babylon.js,three.js etc)
- Cocos(can publish H5)
- Unity(WebGL)

I need to do a good analysis and decide which engine to use.