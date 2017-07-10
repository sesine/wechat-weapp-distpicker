# 微信小程序地区选择器

微信小程序自带了时间选择器、日期选择器，但是没有地区选择器。

:mask:于是只能撸代码撸了一个出来

## 展现方式

有两种方式可以选择：

- picker 普通选择器方式（分成三个选项）

- picker-view 滚动选择器方式（三个选项合并成一个）

## 输出数据

数据使用` form `表单进行提交，对各项内容进行了校验，以下条件通过才可提交（不过你可以自己改）

- 各选项值不能为空

- 姓名必须为中文名

- 手机号码格式正确

如果所有条件通过，会在` console `打印表单的数据，然后可以进行之后的操作

输出的数据可以是中文的地区名称` 北京 `，也可以是地区编码 ` 110000 `

切换方法：在wxml页面文件中，` {{provinceName[provinceSelIndex]}} `为地区名称，如果改成` {{provinceCode[provinceSelIndex]}} `就是地区编号

> 数据存在隐藏的input中（如果直接使用input会唤起键盘）



---

这是效果图：

![poster](https://static.sesine.com/wechat-weapp-distpicker/poster.jpg)

如果喜欢的话，请star:blush:
