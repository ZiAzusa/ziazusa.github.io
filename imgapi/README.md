# Nahida.Fun随机二次元图片API使用说明
本随机图API基于[MirlKoi图库](https://iw233.cn)的公开数据打造，图片绿色健康，无NSFW内容<br>
使用我自建的图床服务，避免了新浪图床报403的问题<br>
### 食用方法
API地址：https://imgapi.nahida.fun<br>
调用方法：GET<br>
#### 传入参数说明：
| 键 | 键描述 | 值类型 | 可用的值 | 值描述 |
| --- | --- | --- | --- | --- |
| sort | 索引的图片集 | Text | random<br>top<br>cat<br>yin<br>xing<br>mp<br>pc | 索引全部图片<br>索引精选图片 (3951P)<br>索引兽耳图片 (2515P)<br>索引银发图片 (2071P)<br>索引星空图片 (526P)<br>索引竖屏壁纸 (1828P)<br>索引横屏壁纸 (1083P) |
| type | 输出方法<br>(可选，默认为重定向) | Text | text<br>json | 输出文本<br>输出JSON格式 |
| num  | 输出图片数量<br>(可选，当num大于等于2时type固定为json) | Number | 大于等于1,小于等于100的任意整数值<br>若不携带num则默认为1 |   |

Demo：<br>
```
GET https://imgapi.nahida.fun/?sort=random
GET https://imgapi.nahida.fun/?sort=top&type=json
GET https://imgapi.nahida.fun/?sort=cat&num=100
```
#### 返回参数说明：
注意：当携带num参数且num参数大于等于2时，API只会输出JSON格式
| 传入type | 返回值 | Demo |
| --- | --- | --- |
| text | 图片URL | ```https://img.moeloli.cyou/2023/01/02/63b2fb7ed3537.jpg``` |
| json | {"pic": 图片URL(s)数组} | ```{"pic": ["https:\/\/img.moeloli.cyou\/2023\/01\/02\/63b2fb7ed3537.jpg"]}``` |
| 其它 | 重定向到图片URL | ```header("Location: https://img.moeloli.cyou/2023/01/02/63b2fb7ed3537.jpg")``` |
