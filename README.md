# Voice-extractor-based-on-Whisper-and-WavLM
本项目用于生成语音训练集
## 只有一个角色时:<br>
![image](https://user-images.githubusercontent.com/42380934/222331950-c40d03e4-e16c-4d69-b5fa-c79b8a8c459d.png)
<br>将STT.ipynb中的pth改为原音频文件路径<br>
运行STT.ipynb在文件夹slices中生成语音切片, 同时生成对应文本list.txt
<br>
## 有多个角色时:<br>
![image](https://user-images.githubusercontent.com/42380934/222331950-c40d03e4-e16c-4d69-b5fa-c79b8a8c459d.png)
<br>将STT.ipynb中的pth改为原音频文件路径<br>
运行STT.ipynb在文件夹slices中生成语音切片, 同时生成对应文本list.txt
<br>
![image](https://user-images.githubusercontent.com/42380934/222332318-4c005aff-6529-470c-b9ef-f60698616d05.png)
<br>
在slices中选择5-10个目标角色语音复制到samples/1中
<br>
在slices中选择5-10个非目标角色语音复制到samples/0中
<br>
![image](https://user-images.githubusercontent.com/42380934/222332282-eb696af9-c2b0-4e66-80dd-fa4836667b79.png)
<br>
然后运行classify.ipynb<br>
<br>运行过程中会出现弹窗, 用于半自动增加样本量<br>
![image](https://user-images.githubusercontent.com/42380934/222332912-9f4659e1-5628-46b9-93bc-53822316fd3a.png)
<br>将弹窗播放的每个音频归入正样本(Positive)或负样本(Negative)<br>
<br>大约对100个左右的样本进行归类, 程序就可以得到最终结果, 并保存在result中<br>
![image](https://user-images.githubusercontent.com/42380934/222333416-86df916f-7828-42ee-8345-f4492cf03129.png)
![image](https://user-images.githubusercontent.com/42380934/222333436-261b505e-2b91-46d8-beae-5dbda46e3085.png)
