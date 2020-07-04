# matlab figure

**坐标轴设置**

1. 坐标轴刻度调整

~~~matlab
set(gca,'YTick',0:200:400)%%先设置坐标轴范围
set(gca,'YTick',[0.00006 0.0006 0.006 0.6])
set(gca,'YtickLabel',{'0','200','400'})%%设置坐标轴刻度标签
~~~

2. 坐标轴比例调整

~~~matlab
set(gca,'DataAspectRatio',[200 200 1])%%分别是x y z坐标刻度比例
~~~



**图例**

1. 根据散点颜色添加图例

~~~matlab
h1(1) = plot(x1,y1,'rs');hold on
h1(2) = plot(x2,y2,'gs');hold on
legend([h1(1) h1(2)],'函数1图例','函数2图例',location,best)
~~~

2. 图例位置

```matlab
legend([h1(1) h1(2)],'函数1图例','函数2图例',location,eastoutside)
```

esatoutside可以修改参考**属性检查器——标签——Legend——potion**

**线条属性**

~~~matlab
plot(h1(1),'LineWidth',1)%%宽度
plot(h1(1),'LineStyle','-')%%线型
plot(h1(1),'Color','k')%%颜色
~~~

