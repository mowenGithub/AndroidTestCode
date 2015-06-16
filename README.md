# AndroidTestCode
android的一些测试代码


scaletypetest分支：测试坑爹的scaleType属性

scaleType是fixCenter或centerInside等等属性时，如果图片比较大，虽然会缩放，但其容器ImgeView的高度（也可能是宽度）还是原图片的高度。而使用adjustViewBounds属性则不会出现这种问题，下面是运行后的效果图（上面是用adjustViewBounds，下面是用scaleType=fixCenter）:
![image](https://github.com/mowenGithub/AndroidTestCode/blob/scaletypetest/img/test_result.jpg)