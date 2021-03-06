---
title: SDK更新日志
type: product
order: 2
---

## 2017/11/28

1. [All] GObject.visible修改了底层的实现方式，以前visible=false时是将原生对象移出显示列表的，现在改成不移出，仅仅是设置原生对象的visible=false。
2. [Laya] 更新了例子，使用LayaAir 1.7.12。
3. [Egret] 更新了例子，使用EgretEngine 5.0.13。
4. [Laya] 修正了Base64编码的bug。（影响像素点击测试功能）
5. [Cocos2dx] 正式版发布。
6. [Unity] Unity发布了1.9.2版本。
7. [Unity] 修正了如果UIPanel中有使用倾斜功能。则在编辑模式会报错的bug。
8. [Unity] 修正了如果位图字体有重名时报错的bug。
9. [Unity] 增加了onTouchMove事件。调用context.CaptureTouch后，对象可以收到这个事件（无论鼠标是否在对象上），直到touchEnd。
10. [Unity] 改进了GoWrapper，现在会复制对象的材质，避免造成原始材质的变化。
11. [Unity] 修正了有时当对象销毁后，自动合批出现不正确的bug。
12. [Unity] 增加了对HTML语法的支持，支持设置图片的宽度或高度为百分比，例如width='50%' height='50%'。
13. [Unity] 增加了GTextInput.SetSelection，可以选定输入框中的文字。
14. [Unity] 修正了滚动容器关闭滚动惯性后，item贴近或分页滚动没有正确处理的bug。

## 2017/9/24

1. [All] 修正了虚拟列表滚动后丢失ITEM选中状态的问题。
2. [All] 修正了滚动容器的一个bug，对于设置了贴近ITEM的滚动容器，当滚动时，如果点击停止，停止后没有回到贴近ITEM的正确位置。
3. [Flash/Starling/Egret] 增加了MovieClip的平滑设置支持。
4. [Egret] 修正了富文本点击链接触发两次的问题。
5. [Unity] Unity发布了1.9.0版本。
6. [Unity] 移动平台现在也支持RollOver和RollOut事件了。
7. [Unity] GoWrapper现在可以包装UGUI的Canvas，实现FairyGUI中嵌入UGUI的需求。[使用方法](../guide/unity/insert3d.html#插入Canvas)
8. [Unity] 如果手势是全屏的，也就是没有具体对象的，现在可以直接建立在GRoot上。[使用方法](../guide/unity/input.html#手势)
9. [Unity] 修正了部分输入法，以及在Mac下无法输入中文的bug。
10. [Unity] 修正了字体贴图重建时，没有销毁材质，可能造成内存泄漏的bug。
11. [Unity] GoWapper增加了对sharedMaterial是否为空的判断。
12. [Unity] 如果使用源码版本，不再为移动平台屏蔽OnGUI函数，这会造成不响应按键事件。
13. [Unity] Stage.touchScreen不再只读，现在可以手工改变。
14. [Unity] 对于设置为使用Raycast进行点击测试的UIPanel，现在你可以使用HitTestContext.layerMask排除掉一些不关心的层。