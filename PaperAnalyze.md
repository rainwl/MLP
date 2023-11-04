# 现有技术分析

## 需求

用户为老师或者学生,平台为web(适用于手机,平板,电脑),输入尽可能的简单快捷方便,达到快速检索的功能,并且能够导出特定格式,以及和PPT的深度结合.

### 输入
- 文字
- 拍照
- 草图

大体的设计,我目前思考的大概样子如下,有一个输入栏,作为文字输入,利用文字进行匹配(人工标签,自动化标签),以及还有一个拍照按钮,进行图像识别匹配,以及可以直接在页面上画草图轮廓,进行匹配.

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_3032.PNG" width=20%>

## 论文分析

### 基于多特征融合的三维模型检索的研究

论文首先提出了传统的基于文字标签检索的劣势,然后要进行复杂且自动化的方式,需要用到一些模型的固有属性,几何等特征.

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7976(20231024-001408).PNG" width=80%>

然后提出了三种方案:
- 人工文字标签
- 草图轮廓(难点在于2D转3D表达)
- **输入一个三维模型,然后这个模型与模型库中的模型进行比对检索**

该论文的两种实现,基于视觉的混合方案,以及深度学习方案,全是基于最后一种模型与模型比对的.

从需求层面而言,是不方便最初定义的网页端,输入文字,拍照,草图的简便形式的.

所以该论文针对于本模型库项目可提供的实际价值不是很大.可以借鉴学习里面的一些概念.


<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7977(20231024-001431).PNG" width=80%>

比如三维模型的特征提取方法,这些具有一定的借鉴学习价值.

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7978(20231024-001506).PNG" width=80%>

然后这个体素化+卷积神经网络的方式,可以简单借鉴下体素,看看特征的提取.其他针对于模型库的需求上价值不是很大.

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7979(20231024-001540).PNG" width=80%>

综上,该论文主要实现了两种,通过输入模型,去和模型库里的模型进行比对的方法,对于web端的快速检索需求而言,只能起到一定借鉴价值,无法实际直接使用,需求层面存在偏差.

### 基于视图和哈希学习的三维模型检索算法研究

该文章,提供了一个web界面,其中涉及的web技术值得借鉴和学习,然后给出了两种检索方案,一个是上传图片,一个是上传模型.

上传模型的可以不考虑,然后上传图片,这个可以学习借鉴,这个和拍照识别类似(但是拍照识别和背景复杂度等等还有关系,可能有滤波等操作,复杂环境照片和直接给一个差不多的二维图,还是有点区别).

同时该文章里实现的软件,提供了模型格式转换的功能(调用blender的库),提供了一定的思路,值得学习借鉴.
<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/45977C7049CC615D94E5A3549DE5D4EF.png" width =80% >

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/045E297FD61BAE8CD52B20BA438F8C12.png" width =80% >

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7982.PNG" width =80% >

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/3582060E98A69B4AC738149E860BA9AB.png" width =80% >




<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7989.PNG" width=80%>

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/AEC29201C4901853D6731E091B21957F.png" width=80%>

<img src="https://pic4rain.oss-cn-beijing.aliyuncs.com/img/IMG_7991.PNG" width=80%>


## 结论

两篇论文提到的三维模型检索方案,都包括输入模型,和库中模型做比对的方式.针对文字输入,拍照识别,
草图轮廓匹配的web端三维模型检索库项目,并不是很适合.

但是第二篇论文里,包含了二维图输入检索的功能,值得学习借鉴.

对PPT的深度定制功能在上述两篇论文中没有去实现.

我认为该项目,可能更多的还是通过分析几何特征,量化模型数据,以及计算机视觉方案去做更贴切一些,然后草图轮廓匹配的技术难点更大一些,也可能是最后,最好用的检索方式,可以投入研究.

这两篇文章,可以借鉴的地方也挺多,主要是第二篇可以输入二维图检索匹配那个值得学习,然后他们主要涉及的模型匹配模型的方式,我感觉需求上可能不是太需要.

