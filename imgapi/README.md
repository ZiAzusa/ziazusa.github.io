# MoeLoli随机图使用说明
本随机图API基于[MirlKoi图库（R.I.P.）](https://iw233.cn)的公开数据打造<br>
使用我自建的图床服务，避免了新浪图床报403的问题<br>
### 食用方法
API地址：https://imgapi.moeloli.cyou<br>
调用方法：GET<br>
参数说明：<br>
| 键 | 值类型 | 描述 | 可用的值 |
| --- | --- | --- | --- |
| sort | Text | 选择的图片集 | random 索引：全部图片<br>cat    索引：兽耳图片<br>wh     索引：银发图片<br>mp     索引：竖屏壁纸<br>pc     索引：横屏壁纸 |
| type | Text | 输出方法(可选，默认为302转发) | text 输出文本<br>json 输出JSON格式 |
