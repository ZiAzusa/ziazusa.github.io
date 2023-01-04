# MoeLoli随机图使用说明
本随机图API基于[MirlKoi图库（R.I.P.）](https://iw233.cn)的公开数据打造<br>
使用我自建的图床服务，避免了新浪图床报403的问题<br>
### 食用方法
API地址：https://imgapi.moeloli.cyou<br>
调用方法：GET<br>
#### 传入参数说明：
| 键 | 键描述 | 值类型 | 可用的值 | 值描述 |
| --- | --- | --- | --- | --- |
| sort | 索引的图片集 | Text | random<br>cat<br>wh<br>mp<br>pc | 索引全部图片<br>索引兽耳图片<br>索引银发图片<br>索引竖屏壁纸<br>索引横屏壁纸 |
| type | 输出方法(可选，默认为重定向) | Text | text<br>json | 输出文本<br>输出JSON格式 |
Demo：<br>
```
GET https://imgapi.moeloli.cyou?sort=random
```
#### 返回参数说明：
| 传入type | 返回值 |
| --- | --- | --- |
| text | 图片URL |
| json | {"pic": "图片URL"} |
| 其它 | 重定向到图片URL |
Demo：<br>
```JSON
text:
    https://img.moeloli.cyou/2023/01/02/63b2fb7ed3537.jpg
json:
    {"pic": "https:\/\/img.moeloli.cyou\/2023\/01\/02\/63b2fb7ed3537.jpg"}
其它:
    header("Location: https://img.moeloli.cyou/2023/01/02/63b2fb7ed3537.jpg")
```
