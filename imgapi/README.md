# MoeLoli随机图使用说明
本随机图API基于[MirlKoi图库（R.I.P.）](https://iw233.cn)的公开数据打造<br>
使用我自建的图床服务，避免了新浪图床报403的问题<br>
### 食用方法
API地址：https://imgapi.moeloli.cyou<br>
调用方法：GET<br>
参数说明：<br>
| 键 | 键描述 | 值类型 | 可用的值 | 值描述 |
| --- | --- | --- | --- | --- |
| sort | 索引的图片集 | Text | random<br>cat<br>wh<br>mp<br>pc | 索引全部图片<br>索引兽耳图片<br>索引银发图片<br>索引竖屏壁纸<br>索引横屏壁纸 |
| type | 输出方法(可选，默认为302转发) | Text | text<br>json | 输出文本<br>输出JSON格式 |
