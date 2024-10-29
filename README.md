# 运行方式
下载MAC-pecker.zip，将MAC-pecker.Rmd, MP.RData, uE.Rdata, logo.png解压在同一目录下：

方式一 使用命令执行MAC-pecker.Rmd：

```
R -e "rmarkdown::render('MAC-pecker.Rmd',output_file='output.html')"
```
方式二 使用RStudio打开Rmd文件运行

# 使用说明
![image](https://github.com/user-attachments/assets/f6684206-31ba-47b5-8f35-0d6d3342808a)
运行RMD文件后，进入MAC-Pecker操作界面，界面分为左侧的操作区和右侧的展示区。
使用时先在操作区选择预测方式，选择“MC”以预测一定MC下应达的PC率，选择“PC”以预测一定PC率下的MC率，此处以选择预测方式为“MC”为例展示操作：
首先选择预测方式为“MC”，分别在“定义基线值”、“定义参考值”和“定义目标MC/PC”处选择基线值、参考值和对应的目标MC。
![image](https://github.com/user-attachments/assets/24b7a2b8-148c-4a88-a61f-95131a73de3b)
此处以“World”（即世界水平的MC覆盖率和阴茎癌发病率）作为基线值，以“Brazil”（即巴西的MC覆盖率和阴茎癌发病率水平）作为参考值，以“80”（即MC覆盖率为80%）作为目标MC，定义完成后点击“点击计算”，右侧展示区就会展示结果和对应的图像。
![image](https://github.com/user-attachments/assets/fb2fbb69-6eb9-4553-ac1b-d9b1d5b2febb)
展示区上方为结果说明，会用一句话展示预测得到的阴茎癌发病率的值及相应的置信区间；下方为在参考值的MC覆盖率和阴茎癌发病率水平下，模型预测得到的MC覆盖率与阴茎癌发病率累积关联曲线，图上标有95%置信区间和不同世界地理区域与全球185个国家/地区根据2022年HDI划分得到的四分位数组平均MC覆盖率和阴茎癌发病率在图上的对应点。
若选择预测方式为“PC”，其余操作均相同，只是此时需要定义目标PC而非MC，预测得到的是某国家/地区达到一定PC率所需达到的最低MC覆盖率。

# 注意事项
（1）工具使用MC覆盖率为15~49岁男性，阴茎癌发病率为全年龄
（2）预测模型未考虑包茎和HPV感染率的动态变化，而是基于现有情况进行简单估算，即假设当前包茎率和HPV感染率不变进行估算
