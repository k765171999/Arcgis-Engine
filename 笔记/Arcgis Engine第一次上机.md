## Arcgis Engine第一次上机

### 基本C#操作

* 制作程序1+1=2

  > 1. 在用户界面新建C#窗口程序，拖动两个按钮三个文本框到界面，其中的加号、等于可以用label。
  >
  >    ![](E:\学习\Arcgis Engine Git\Github\笔记\img\2018-09-25_164359.png)
  >
  > 2. 在属性中可以更改按键上的名字，以及这个按钮的名字。
  >
  > 3. 选中界面中的一个按钮，点击事件，选到click。
  >
  >    ![](E:\学习\Arcgis Engine Git\Github\笔记\img\2018-09-25_164712.png)
  >
  > 4. 在代码区域编辑代码（注意类型之间的转换！）。
  >
  >    ```c#
  >       			string input1 = textinput1.Text;
  >                string input2 = textinput2.Text;
  >
  >                int intinput1 = Convert.ToInt32(input1);
  >                int intinput2 = Convert.ToInt32(input2);
  >
  >                //int resulttmp = ClassLibrary1.addClass(intinput1, intinput2);
  >                ClassLibraryAdd.addClass addsss = new ClassLibraryAdd.addClass();
  >                int resulttmp = addsss.add(intinput1, intinput2);
  >                //int resulttmp = add(intinput1, intinput2);
  >    			//convert可以强制转换
  >                string result = Convert.ToString(resulttmp);
  >
  >                textresult.Text = result;//XXXX.Text可以获得，或者改变文本框中的东西
  >    ```
  >
  >    ​

* 运用类库

  > 1.  先新建一个类库。
  >
  > 2. 在类中添加方法。
  >
  > 3. 生成解决方案。
  >
  > 4. 在上一步的**引用**中选择->添加引用->浏览，在bin中选择到dll。
  >
  >    ![](E:\学习\Arcgis Engine Git\Github\笔记\img\2018-09-25_165258.png)
  >
  > 5. 回到上一步代码中实例化类库。
  >
  >    ```c#
  >    ClassLibraryAdd.addClass addsss = new ClassLibraryAdd.addClass();
  >    ```
  >
  >  6. 正常编辑运行。

