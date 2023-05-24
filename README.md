# langchain-wiki
基于langchain开发的知识库，一步步教你入手大模型开发，即使您是一个门外汉也能轻松入门。

本项目旨在教您如何快速入手大模型开发。项目的目标是通过结合当前热门的langchain技术，为您展示如何迅速构建类似"New Bing"效果的知识库应用。

为了担心项目复杂度太高，我们特别为您准备了一个使用Python脚本实现所有功能的教程，而且我们会在知识星球上逐行解说实现过程。此外，我们还会不定期进行直播，分享与该技术相关的实际应用。无需担心自己的背景知识，我们将用简洁易懂的方式，引导您快速掌握大模型开发的技巧，并拓宽自己的知识领域。

欢迎您加入我们的知识星球，并与我们一起交流。在我们的知识星球中，您将获得以下益处：
* 手模手带您入门大模型的应用开发，逐行讲解实现的过程
* 定期分享大模型开发的实践项目和资源
* 与志同道合的人一起学习和进步
* 其他开发者合作创造令人惊叹的作品

不再只是门外汉，加入我们的行列，一起窥探大模型的奥秘！
![xingqiu](resources/xingqiu.jpg)

## 快速开始

下载或者克隆此github仓库
```bash
git clone git@github.com:llm-ai-dev/langchain-wiki.git
```

用conda创建个虚拟环境并激活
```bash
conda create -n langchain-wiki python=3.10 -y
conda activate langchain-wiki
```

进入项目并安装依赖包
```bash
cd langchain-wiki
pip install -r requirements.txt  
```

因为是基于openai开发的，所以需要修改当前项目下的.env文件，设置key
```bash
OPENAI_API_KEY=填写您的openai的密钥
```

需要使用openai的api，这里需要您设置下代理地址，确保您可以访问openai
```
export https_proxy=填写您的代理地址 http_proxy=填写您的代理地址
```

**启动 Web 界面**
启动后，您将可以在终端看到访问的地址，这里我们也对手机上的UI做了优化，欢迎体验
```
# 默认gradio可以访问启动路径下的所有文件，所以这里建立一个app目录用于启动脚本，防止一些敏感文件泄漏
cd ./app
python ./main.py
```
初始用户名和密码：admin, wikidb@123.com

注意：如果您不想公开，可以自行修改`main.py`，把demo.launch中share修改为False
## 效果演示
视频生成GIF效果和样式有点失真，后续会上传到b站供大家观看
![web-demo](resources/web-demo.gif)

## 免责声明
请各位严格遵守如下约定：
1. 本项目任何资源仅供学术研究使用，严禁任何商业用途。
2. 本项目不承担任何法律责任，亦不对因使用相关资源和输出结果而可能产生的任何损失承担责任。
