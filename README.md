# 🤖 ChatGPT-Assistant
基于Streamlit搭建的ChatGPT聊天界面，简单易用，支持以下功能：
- 多聊天窗口
- 历史对话留存
- 预设聊天上下文 
- 模型参数调节

# 部署
## 本地部署
1. 建立虚拟环境（建议）

2. 复制项目
```bash
git clone https://github.com/PierXuY/ChatGPT-Assistant.git
```

3. 安装依赖
```bash
pip install -r requirements.txt
```

4. 设置API Key   

- 在 `.streamlit/secrets.toml`文件中写入`apikey = "Your Openai Key"`

5. 启动应用
```bash
streamlit run app.py
```

## 云平台部署


# 说明
- 在[helper.py](https://github.com/PierXuY/ChatGPT-Assistant/blob/main/helper.py)文件中可自定义用户名和SVG格式[头像](https://www.dicebear.com/playground?style=identicon)。
- 在自己部署的项目中编辑**set_context.py文件**，即可增加预设定的上下文选项，会自动同步到应用中。
- 在[Streamlit Cloud](https://docs.streamlit.io/streamlit-community-cloud/get-started)或者[Hugging Face](https://huggingface.co/)可免费部署，且无须科学上网即可使用。
- 在Hugging Face部署时，如果更新应用会造成历史对话丢失，有条件的可以把help.py文件中的读写逻辑改为数据库读写，永久保留数据。

# 致谢
- 最早是基于[shan-mx/ChatGPT_Streamlit](https://github.com/shan-mx/ChatGPT_Streamlit)项目进行的改造，感谢。
- [预设的上下文话术](https://github.com/PierXuY/ChatGPT-Assistant/blob/main/set_context.py)参考自[binary-husky/chatgpt_academic](https://github.com/binary-husky/chatgpt_academic)项目和[f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)项目，感谢。
