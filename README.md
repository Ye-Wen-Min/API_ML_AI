# API_ML_AI PRD
* 史诗：知你 
* 目标版本：2018年12月 
* 发布日期：2018年11月25日
* 文件状态：进行中
 * 文件的主人：叶文敏
* 领头的设计师：叶文敏 
 * 领头的开发者：叶文敏
* 领头的测试者：叶文敏

## 用户案例：
* 将会议记录语音转为文本笔记，你的专属工作秘书。（短需求）
## 目标：
* 知你小程序将会议上的音频转换为文字记录，节省人力和时间成本，具有云工作室功能，方便工作协作，具有任务进程打卡功能，工作进度一目了然，摆脱工作拖延症。

## 背景和战略契合：

### 背景：

* 面对繁杂的会议记录依靠听当场记录或者后期听录音人工记录耗费大量的人力和时间，人工记录的准确度尚有所偏差，运用会议记录即时转文本功能可以即时高效转化；工作族总有拖延症的习惯和漏看通知的习惯，云工作室的功能包含发布工作通知，进行工作进度打卡，有利于针对性地改变拖延症和提高工作信息获取度。

### 战略契合：
* 需要运用到智能长语音识别和语音理解的功能，将会议上的音频转换为文字信息，方便后期的文字处理和内容存档。小程序相对输入法中带有该功能的APP来说比较强轻量级、偏向商务工作性质，容易吸引商务一族使用，增加用户粘性。


## 假设：
### 用户假设：
* （1）用户需要准备一部智能手机，点开知你小程序。
* （2）打开手机的录音权限，允许音频的录入。
* （3）需要联网。
### 技术假设：
* （1）开启手机录音权限，启用手机麦克风录音。
* （2）运用长语音识别API将录音转为文字。目前在线识别支持普通话、英文、粤语和四川话。
* （3）进行机器学习中语义理解：将语音识别出的文字，进行分词及找出意图。



## 用户需求：


| 短标题 | 用户故事 | 重要性 | 
| - | :-: | -: | 
| 办公小白 | 高效完成会议记录的转换并记录，提高个人的工作效率，减少日夜加班的状况，减缓拖延症带来的DDL压力。| 很重要| 
| 工作领导者 | 想要对会议记录进行自我的收藏以及存档，方便下一次开会准备| 重要 |
 

## 使用者交互以及设计：
### 产品功能结构图：
![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/img/%E7%9F%A5%E4%BD%A0%E5%B0%8F%E7%A8%8B%E5%BA%8F.png)

### 产品流程图：
![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/img/%E6%B5%81%E7%A8%8B%E5%9B%BE%20(1).png)

### 产品信息结构图：
![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/img/%E7%9F%A5%E4%BD%A0%E5%B0%8F%E7%A8%8B%E5%BA%8F2.png)


### 交互界面设计：

##  [ 原型文档仓库URL](https://ye-wen-min.github.io/API_axure/index.html
 )

![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/%E7%95%8C%E9%9D%A2/%E9%A6%96%E9%A1%B5%E6%8E%88%E6%9D%831.png)

### 首页授权界面
* （1）微信点开授权登录小程序。
* （2）点击获取麦克风授权。
* （3）底部导航栏有会议记录转换、云公作作室和我的功能。




![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/%E7%95%8C%E9%9D%A2/%E4%BC%9A%E8%AE%AE%E8%AE%B0%E5%BD%95%E8%BD%AC%E5%8C%96%E9%A1%B5%E9%9D%A2.png)

## 会议记录转换
* （1）点击新建笔记，则新建一则笔记文档。
* （2）会议记录列表中选中选框后，跳转至编辑该会议记录页面。
* （3）点击开始录译则开始会议记录的实时音频转换为文本功能，具有保存、编辑、分享按钮可选择。
* （4）显示总记录时长。



![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/%E7%95%8C%E9%9D%A2/%E4%BC%9A%E8%AE%AE%E8%AE%B0%E5%BD%95%E8%BD%AC%E5%8C%96%E9%A1%B5%E9%9D%A2.png))

## 任务列表
* （1）新建任务可对任务进行编辑。
* （2）任务列表可看到任务完成度，也可对任务每日进行打卡。




![img](https://github.com/Ye-Wen-Min/API_ML_AI/blob/master/%E7%95%8C%E9%9D%A2/%E4%BA%91%E5%B7%A5%E4%BD%9C%E5%AE%A4.png)

## 云工作室
* （1）云工作室具有加入工作室显示、新建工作室、在线协作和会议记录分享功能。




## 问题：

问题 | 结果
---|---
 输入会议音频内容| 输出会议内容文本信息
输入任务内容以及期限|输出任务打卡进度条和倒计时



## 超范围功能：
* 用户会议内容进行社交化的分享，对会议记录有评论以及点赞等交互。

## 加值宣言

* 知你小程序将会议上的音频实时转换为文字记录的这一核心功能调用了百度AI的专业语音识别的API。其中语音识别及长语音识别SDK内部均为采用流式协议，即用户边说边处理。区别于Rest api需要上传整个录音文件。故用户可以实时通过对会议现场的录音获取会议的文本内容。

## 核心价值

* 产品的预期核心价值是将会议上的音频实时转换为文字记录，实现会议记录高效实时更新。这是最小可用产品，提高了用户商务工作的高效性，初步完成了产品是用户的个人工作助手的部署。

## 核心价值与用户痛点

* 产品核心价值是对会议的音频实时转化为文本文件可以方便后期查看和编辑，产品solgan为成为陪伴你成长的工作小秘书。这解决了用户以下痛点：
* （1）在开会时，面对繁多的会议内容，当场记录难度大，准确度低。
* （2）在开会之后，对会议内容的后期记录工作量繁重，有时需要付出大量的时间才能完成。

### 人工智能概率性与用户痛点
* 百度拟开放人工智能技术语音识别准确率达97%：
[据悉，百度基于深度学习研发的新一代深度语音识别系统识别准确率可达到97%。](http://www.sohu.com/a/113334468_119536)
* 知你小程序将会议上的音频实时转换为文字记录的这一功能调用了语音识别的API。在线识别转换为普通话、英文、粤语和四川话等语种，转化精确率较高，普遍情况下都可以使用。该产品因环境因素或者语音语调造成识别不准确的状况，转换概率较小为少数事件，对正面影响并不，基本能解决对会议内容等的实时记录的用户痛点。

## 需求列表与人工智能API加值（可行性）

* 明确需求：会议语音转换文本功能，面对的人群主要是处理日常商务工作上班一族，针对的场景是会议记录的现场，解决的问题是不用耗费大量时间在记录会议内容上。
* 现有功能为：会议语音转换文本，运用百度语音识别API中长语音识别，通过SDK调用服务，可将长语音（长时间连续说话）转换为文字。

###  API运用
#### 百度API
* 百度AI的专业语音识别的API。其中语音识别及长语音识别SDK内部均为采用流式协议，即用户边说边处理。区别于Rest api需要上传整个录音文件。
* 接口描述：向远程服务上传整段语音进行识别 ，输入音频文件，输出文本信息。
* 接口地址以及SDK调用：
* AipSpeech是语音识别的Python SDK客户端，为使用语音识别的开发人员提供了一系列的交互方法。
参考如下代码新建一个AipSpeech：

```
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '你的 App ID'
API_KEY = '你的 Api Key'
SECRET_KEY = '你的 Secret Key'

client = AipSpeech(APP_ID, API_KEY, SECRET_KEY)

```
* 请求说明
要对段保存有一段语音的语音文件进行识别：

```
# 读取文件
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

# 识别本地文件
client.asr(get_file_content('audio.pcm'), 'pcm', 16000, {
    'dev_pid': 1536,
})
```
* dev_pid 参数列表：


dev_pid | 语言
---|---
1536 | 普通话(支持简单的英文识别)
1537 | 普通话(纯中文识别)
1737 | 英语
1637 | 粤语
1837 | 四川话
1936 | 普通话远场

* 返回样例：
```
// 成功返回
{
    "err_no": 0,
    "err_msg": "success.",
    "corpus_no": "15984125203285346378",
    "sn": "481D633F-73BA-726F-49EF-8659ACCC2F3D",
    "result": ["北京天气"]
}

// 失败返回
{
    "err_no": 2000,
    "err_msg": "data empty.",
    "sn": null
}

```
* 我们只需利用requests模块发送post请求到拼出来的url就可以了。

```
import requests

#获取tokent
baidu_server = "https://openapi.baidu.com/oauth/2.0/token?"
grant_type = "client_credentials"
#API Key
client_id = "xxxx"
#Secret Key
client_secret = "xxxx" 

#拼url
url ="%sgrant_type=%s&client_id=%s&client_secret=%s"%(server,grant_type,client_id,client_secret)
print(url)
#获取token
res = requests.post(url)
print(res.text)
token = json.loads(res.text)["access_token"]
print(token)
#24.b891f76f5d48c0b9587f72e43b726817.2592000.1524124117.282335-10958516import requests

#获取tokent
baidu_server = "https://openapi.baidu.com/oauth/2.0/token?"
grant_type = "client_credentials"
#API Key
client_id = "qRHV7hrxj8vtAGuZOpG0zW58"
#Secret Key
client_secret = "Bg3Bmx3uPeCUnvuHxnS16HLnNiVPuPnz" 

#拼url
url ="%sgrant_type=%s&client_id=%s&client_secret=%s"%(server,grant_type,client_id,client_secret)
print(url)
#获取token
res = requests.post(url)
print(res.text)
token = json.loads(res.text)["access_token"]
print(token)
#24.b891f76f5d48c0b9587f72e43b726817.2592000.1524124117.282335-10958516
```



