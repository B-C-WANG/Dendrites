# Dendrites
## Preview 预览
- Numpy in dendrites 在dendrites中使用numpy进行矩阵操作
![](/doc_image/9.png)
- Pandas in dendrites 在dendrites中使用pandas处理表格数据
![](/doc_image/10.png)

- Dendrites is a **visualized flow-based programming** tool for Python, it is **highly customizable** that every function in python can be made to a "Block" with input params as "Pin". It is very similar to the **"Blueprint" in Unreal Engine 4**. Extend basing on Persimmon([https://github.com/AlvarBer/Persimmon](https://github.com/AlvarBer/Persimmon)).With lots of new function and supprting for numpy, pandas, ... dendrites is aimed to help build and test machine learning model ASAP.（dendrites是一个可视化的、基于流式编程的python工具，任何python函数可以作为运行图的一个节点Block，而函数输入输出是作为Block的pin。这种概念已经在很多领域中应用，比如Unreal游戏引擎中的“蓝图”系统。本软件基于Persimmon已有基础进行开发，做了大量的改进，并添加numpy，pandas，sklearn等支持用于构建一个快速机器学习模型评估的工具。）  
![](/doc_image/1.png)
- The function lib of dendrites, called **Dendrites_lib**, is highly customizable and can be imported to Dendrites as a block, e.g.(任何一个函数可以写入dendrites的lib中，从而变为一个block使用):  
![](/doc_image/2.png)
- It has a strict but flexible type system to control the connection of pins using list and "+". Each pin use a list of string to indicate which type of data can be connected to. For example, a type of ["int","float"] means the input pin can connected to the output pins with "int" or "float", an input pin with type of ["array+shape=(-1,16,16)"] can not accpet the output pin of type ["array"], but the output pin with type ["array+shape=(-1,16,16)"] can connect to the input pin with type ["array"]（严格而又自由的类型检查系统，用于限制pin的链接，类型使用list实现“或”，用+号实现“且”。比如，允许数字表示的pin输入，可以写为["int","float"]。类型检查是有方向的，比如一个["array+shape(16,16)"]（代表16x16形状的矩阵）能够传递参数到["array"]的pin，但是反过来不行（+号代表了类型的且，像List\<str\>可以表示为"List+str"））.
![](/doc_image/3.png)
- With a smart block search system, you can easily find what blocks you want.（block搜索功能，利用字符串的相似程度(欧氏距离)搜索block）
![](/doc_image/4.png)
- You can use W A S D to move the blackboard for more space to connecting blocks(使用WASD移动画板得到无限大的放置空间，之后会有缩放功能)
- Easily to import and delete function library. Just copy or delte the files startswith "dendritesLib_" in the folder "dendritesLib"（block库管理：只需要在程序根目录下的dendritesLib文件夹中放入以dendritesLib\_开头的.py文件，即可导入Blocks）  
![](/doc_image/5.png)
- Support for showing out block error information, parallel print block, and embedded block print function.（运行时可显示出现bug的block，可调用多个print block显示内容，以及Block自带运行时显示的功能）
![](/doc_image/6.png)
- Load and Save system (存储和读取Block)
![](/doc_image/7.png)

## How to get dendrites? 如何获得dendrites？
- Dendrites will release as long as it finished. Keep Watching! Your star will encourage this project.（dendrites正在开发中并会在完成时放出，请保持关注，你的star能够鼓励项目的进行）

