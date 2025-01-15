# 1.需求分析
</br>
> 用户登录与注册: 通过手机号登录的方式获取验证码登录app。
> 单词记忆挑战:  用户点击开始测试按钮，根据英文单词和语句提示，在四个中文意思中选取最符合的一个作为答案。模块会根据用户的选择记录准确率、用时、答题进度和单词个数（默认十个）。
> 打卡圈功能: 打卡圈是一个社区交流平台，用户可在其中查看自己和他人的挑战结果。用户可以点赞他人的打卡记录，分享学习心得和经验，形成良好的学习氛围。同时，可设置打卡圈的排行榜，根据用户的挑战得分、连续打卡天数等指标进行排名，激发用户的竞争意识和学习动力。  

# 2.程序设计

## 2.1 网络模块
 使用axios封装HTTP的服务，在页面处导入js访问函数以实现登录，存储，答题，同步打卡圈等交互功能。

## 2.2 登录系统
</br>
 > 用户在操作前需要登陆以保存用户相关信息（提示登陆后跳转）。
 > 填写手机号，获取验证码后填入即成功登录。
 > 由于用户使用手机号登录，所以无需注册模块，如果为首次登录系统自动会保存相关的用户信息。

## 2.3 背单词系统
</br>
 > 理论上使用不同的单词书（包括不同语言）就能移植实现不同语言的单词记忆，本项目中仅仅采用英语四级词书作测试。
 > 根据英文单词并结合语句上下文猜测出中文意思，正确则答对数加一，错误则显示正确答案后跳下一题。最终完成挑战得到最终结果，其中统计结果包含确率、用时等。

![](https://cdn.nlark.com/yuque/0/2025/png/46197141/1736927569096-96f3c7dc-7fa6-48c4-a79d-c8a317159a72.png)

## 2.4 打卡系统
 </br>
  > 完成挑战后可选择同步打卡系统，在用户登录后可以看到不同的挑战者的成绩，可以根据用时或者正确率排序得到排行榜。
  > 用户可以点赞或者评论不同用户的打卡信息，也可以看到自己上传的记录。

![](https://cdn.nlark.com/yuque/0/2025/png/46197141/1736927486765-97bd4ff0-819c-41ee-b5fe-75e3e31e46b4.png)
