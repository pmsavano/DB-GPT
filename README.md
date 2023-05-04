# DB-GPT
A Open Database-GPT Experiment

![GitHub Repo stars](https://img.shields.io/github/stars/csunny/db-gpt?style=social)

[DB-GPT](https://github.com/csunny/DB-GPT) 是一个实验性的开源应用程序，它基于[FastChat](https://github.com/lm-sys/FastChat)，并使用[vicuna-13b](https://huggingface.co/Tribbiani/vicuna-13b)作为基础模型。此外，此程序结合了[langchain](https://github.com/hwchase17/langchain)和[llama-index](https://github.com/jerryjliu/llama_index)基于现有知识库进行[In-Context Learning](https://arxiv.org/abs/2301.00234)来对其进行数据库相关知识的增强。它可以进行SQL生成、SQL诊断、数据库知识问答等一系列的工作。 


## 项目方案
![](ttps://github.com/csunny/DB-GPT/blob/dev/asserts/pilot.png)

[DB-GPT](https://github.com/csunny/DB-GPT) is an experimental open-source application that builds upon the [FastChat](https://github.com/lm-sys/FastChat) model and uses vicuna as its base model. Additionally, it looks like this application incorporates langchain and llama-index embedding knowledge to improve Database-QA capabilities. 

Overall, it appears to be a sophisticated and innovative tool for working with databases. If you have any specific questions about how to use or implement DB-GPT in your work, please let me know and I'll do my best to assist you.

Run on an RTX 4090 GPU (The origin mov not sped up!, [YouTube地址](https://www.youtube.com/watch?v=1PWI6F89LPo))
- 运行演示

![](https://github.com/csunny/DB-GPT/blob/dev/asserts/演示.gif)


- SQL生成示例
首先选择对应的数据库, 然后模型即可根据对应的数据库Schema信息生成SQL

<img src="https://github.com/csunny/DB-GPT/blob/dev/asserts/SQLGEN.png" width="600" margin-left="auto" margin-right="auto" >

- 数据库QA示例 

<img src="https://github.com/csunny/DB-GPT/blob/dev/asserts/DB_QA.png" margin-left="auto" margin-right="auto" width="600">

# Install
1. 基础模型下载
关于基础模型, 可以根据[vicuna](https://github.com/lm-sys/FastChat/blob/main/README.md#model-weights)合成教程进行合成。 
如果此步有困难的同学，也可以直接使用[Hugging Face](https://huggingface.co/)上的模型进行替代。 替代模型: [vicuna-13b](https://huggingface.co/Tribbiani/vicuna-13b)

2. Run model server
```
cd pilot/server
python vicuna_server.py
```

3. Run gradio webui
```
python webserver.py 
```

# Featurs
- SQL-Generate
- Database-QA Based Knowledge 
- SQL-diagnosis

总的来说，它是一个用于数据库的复杂且创新的AI工具。如果您对如何在工作中使用或实施DB-GPT有任何具体问题，请联系我, 我会尽力提供帮助, 同时也欢迎大家参与到项目建设中, 做一些有趣的事情。