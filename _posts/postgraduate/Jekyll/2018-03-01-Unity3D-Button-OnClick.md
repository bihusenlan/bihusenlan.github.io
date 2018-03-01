---
layout: post
title: "Button按钮添加OnClick()监听事件"
data: 2018-03-01 15:27:00 +0800
categories: 研究生涯
tag: Jekyll
---
* content
{:toc}
 
当我们设置GUI时，通常要为Button按钮添加OnClick()监听事件，下面就一起学习吧。
#### 1 创建一个Button按钮，自动生成GUI面板，再创建任意一个C#脚本
>它继承自MonoBehaviour类,其中有我们将要被激活的 OnbtlClick()方法。


    public class UGUIOnClick : MonoBehaviour {
	    // Use this for initialization
	    void Start () {
	        
	    }
	        // Update is called once per frame
	    void Update () {
	        
	    }
	    public void OnbtlClick(){
	        Debug.Log ("On Click Me");
	    }
    } 


---

#### 2 将”UGUIOnClick.cs”挂载到Canvas对象上<br>

![gitment]({{ '/_Photo/works/Button_OnClick2.png' | prepend: site.baseurl }})

![enter image description here](/_Photo/works/Button_OnClick2.png)

---

#### 3 单击Button组件On Click()下方的”+”，给监听列表添加一个事件<br>
<img src="/_Photo/works/Button_OnClick2.png" alt="倪明小站">


---

#### 4 将挂载有UGUIOnClick.cs脚本的游戏对象Canvas拖到下面选框中<br>
<img src="/_Photo/works/Button_OnClick.png" alt="倪明小站">

---

#### 5 展开No Function字样的下拉框，选择UGUIOnClick/Onbt1Click<br>
<img src="/_Photo/works/Button_OnClick3.png" alt="倪明小站">

---


#### 6 一个按钮的触控事件完成，只要我们点击Button，Onbt1Click()方法便提示我们点击了一次"On Click Me".
