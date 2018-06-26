
- 学习没有用过的api

```
    //第一个参数是进行时间的百分比， 第二个参数是值
    Keyframe keyframe1 = Keyframe.ofFloat(0 , 0);
    Keyframe keyframe2 = Keyframe.ofFloat(0.7f , 100);
    Keyframe keyframe3 = Keyframe.ofFloat(1 , 80);

    PropertyValuesHolder progress = PropertyValuesHolder.ofKeyframe("progress", keyframe1, keyframe2, keyframe3);

    ObjectAnimator.ofPropertyValuesHolder(view , progress).setDuration(1000).start();
```

![](images/icon.png)

HenCoder 绘制 7 属性动画 练习项目
===

### 这是什么？

这不是一个独立使用的项目，它是 [HenCoder Android 开发进阶：UI 1-7 属性动画（进阶篇）](http://hencoder.com/ui-1-7) 的配套练习项目。

### 怎么用？

项目是一个可以直接运行的 Android App 项目，项目运行后，在手机上打开是这样的：

![](images/preview.png)

工程下有一个 `/practice` 目录：

![](images/project_practice.png)

你要做的是就是，在 `/practice` 下的每一个 `PracticeXxxView.java` 文件中写代码，绘制出和页面上半部分相同的效果。就像这样：

![](images/preview_after.png)

> 当然，没必要做得和示例一毛一样。这是一个练习，而不是一个超级模仿秀，关键是把技能掌握。

如果做不出来，可以参考 `/sample` 目录下的代码：

![](images/project_sample.png)

练习做完，这期的内容也就掌握得差不多了。
