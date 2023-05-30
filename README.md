# react 图片渐进的加载

### 条件
#### 原图cdn地址是七牛云或者oss

### 组件参数props介绍
#### 

名称 | 类型 |	默认值 | 描述
--- | --- | --- | ---
wrapperClassName | String | |组件外层样式，必须定义宽度，低倍图过渡效果动画才有
className |	String | |img图片样式
src |	String | | 图片地址
delayTime |	number |	1	| 过渡动画持续时间，单位秒
beforeLoad | Function| | img加载后回调
onClick |	Function| | imx点击事件
errorImgUrl |	String | | 图片加载失败后，显示的图片
loading	| "lazy" 、 "eager"	| lazy	| 图片加载模式，lazy懒加载，eager同步加载
quality	| number	| 85	| 图片压缩质量，0-100区间
imageLoadType |"oss","qiniu" | oss | cdn类型