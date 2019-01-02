# Dendrites
## 1 miute to dendrites
- Dendrites is a **visualized flow-based programming** tool for Python, it is **highly customizable** that every function in python can be made to a "Block" with input params as "Pin". It is very similar to the **"Blueprint" in Unreal Engine 4**. Extend basing on Persimmon([https://github.com/AlvarBer/Persimmon](https://github.com/AlvarBer/Persimmon))， dendrites is a very customizable tool for flow-based programming in Pyhon.   
![](/doc_image/1.png)
- The function lib of dendrites, called **Dendrites_lib**, is highly customizable and can be imported to Dendrites as a block, e.g.:  
![](/doc_image/2.png)
- It has a strict but flexible type system to control the connection of pins using list and "+". Each pin use a list of string to indicate which type of data can be connected to. For example, a type of ["int","float"] means the input pin can connected to the output pins with "int" or "float", an input pin with type of ["array+shape=(-1,16,16)"] can not accpet the output pin of type ["array"], but the output pin with type ["array+shape=(-1,16,16)"] can connect to the input pin with type ["array"].
![](/doc_image/3.png)
- With a smart block search system, you can easily find what blocks you want.
![](/doc_image/4.png)
- You can use W A S D to move the blackboard for more space to connecting blocks
- Easily to import and delete function library. Just copy or delte the files startswith "dendritesLib_" in the folder "dendritesLib"  
![](/doc_image/5.png)
- Support for showing out block error information, parallel print block, and embedded block print function.
![](/doc_image/6.png)
- Load and Save system  
![](/doc_image/7.png)
## How to get dendrites?
- Dendrites will release as long as it finished. Keep Watching! Your star will encourage this project.

