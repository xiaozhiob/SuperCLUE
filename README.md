# SuperCLUE

中文通用大模型综合性基准SuperCLUE

<a href='https://www.superclueai.com' target="__blank">SuperCLUE最新9月榜单</a>

文章地址：<a href='https://www.cluebenchmarks.com/superclue.html' target="__blank">www.cluebenchmarks.com/superclue.html</a>

技术报告：<a href='https://arxiv.org/abs/2307.15020' target="__blank">SuperCLUE: A Comprehensive Chinese Large Language Model Benchmark</a>
【2023-10-24】 <a href='https://www.cluebenchmarks.com/superclue_agent.html' target="__blank">SuperCLUE-Agent：Agent智能体中文原生任务评估基准</a>
【2023-9-12】 <a href='https://github.com/CLUEbenchmark/SuperCLUE-safety' target="__blank">SuperCLUE-Safety：中文大模型多轮对抗安全基准</a>



【9月26日】，SuperCLUE发布中文大模型9月榜单。

SuperCLUE是一个综合性大模型评测基准，本次评测主要聚焦于大模型的四个能力象限，包括语言理解与生成、专业技能与知识、Agent智能体和安全性，进而细化为12项基础能力。

相比与上月，新增了AI Agent智能体

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/superclue_idea.jpeg"  width="90%" height="90%"></img>

### SuperCLUE能力评估结构图
<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/category09.png"  width="60%" height="60%"></img>

### SuperCLUE多维度测评方案
<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/superclue_mlitisystem.png"  width="90%" height="90%"></img>


### 为什么新增AI Agent智能体能力？

AI agent（智能体）是当前与大语言模型相关的前沿研究热点，拥有类似贾维斯等科幻电影中人类超级助手的能力，可以根据需求自主的完成任务。
然而，面向AI agent智能体，缺乏针对中文大模型的广泛评估。为了解决这一问题，我们在SuperCLUE新的榜单中新增了AI agent智能体能力的测评。
这个榜单将重点评估AI agent在【工具使用】和【任务规划】两个关键能力上的表现，这项工作旨在为评估中文大模型作为智能体的表现提供一个基础和可能。

### SuperCLUE总排行榜（2023年9月）

| 排名 | 模型 | 机构 | 总分 | OPEN<br/>多轮开放问题 | OPT<br/>客观题 | 许可 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| - | GPT4 | OpenAI | 83.2 | 84.28 | 81.58 | 闭源 |
| - | gpt-3.5-turbo | OpenAI | 63.74 | 61.82 | 66.61 | 闭源 |
| - | Claude2 | Authropic | 62.98 | 60.57 | 66.6 | 闭源 |
| 🏅️ | SenseChat 3.0 | 商汤科技 | 62.75 | 54.29 | 75.45 | 闭源 |
| 🥈 | 文心一言(v2.3.1) | 百度 | 62.61 | 53.72 | 75.93 | 闭源 |
| 🥉 | ChatGLM2-Pro | 清华&智谱AI | 62.12 | 54.31 | 73.84 | 闭源 |
| 4 | vivoLM | vivo | 58.29 | 47.67 | 74.21 | 闭源 |
| 5 | Baichuan2-13B-Chat | 百川智能 | 58.03 | 52.45 | 66.4 | 开源 |
| 6 | MiniMax-Abab5.5 | MiniMax | 57.18 | 46.31 | 73.48 | 闭源 |
| 7 | 豆包 | 字节跳动 | 57.13 | 48.65 | 69.86 | 闭源 |
| 8 | Baichuan2-7B-Chat | 百川智能 | 50.11 | 42.28 | 61.86 | 开源 |
| 9 | 讯飞星火(v4.0) | 科大讯飞 | 50.06 | 40.64 | 64.2 | 闭源 |
| 10 | 通义千问(v1.0.7) | 阿里巴巴 | 49.07 | 33.78 | 72 | 闭源 |
| 11 | OpenBuddy-Llama2-70B | OpenBuddy | 44.29 | 30.84 | 64.46 | 开源 |
| 12 | Qwen-7B-Chat | 阿里巴巴 | 40.14 | 23.59 | 64.97 | 开源 |
| 13 | Chinese-Alpaca-2-13B | yiming cui | 39.81 | 32.64 | 50.56 | 开源 |
| 14 | ChatGLM2-6B | 清华&智谱AI | 38.41 | 25.49 | 57.8 | 开源 |
| 15 | ERNIE-3.5-Turbo | 百度 | 37.76 | 24.81 | 57.19 | 闭源 |
| 16 | 360GPT_S2_V94 | 360 | 37.11 | 18.97 | 64.32 | 闭源 |
| - | Llama-2-13B-Chat | Meta | 31.63 | 29.83 | 34.33 | 开源 |

本次评测选取了目前国内外最具代表性的20个通用大语言模型，9月评测数据集为全新的3458道测试题。

### SuperCLUE-OPEN多轮开放问题排行榜（2023年9月）
| 排名 | 模型 | 机构 | OPEN分数 | 语言理解与生成 | 专业技能与知识 | AI智能体 | 安全性 | 许可 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| - | GPT4 | OpenAI | 84.28 | 100 | 90.51 | 91.67 | 81.25 | 闭源 |
| - | gpt-3.5-turbo | OpenAI | 61.82 | 72.22 | 63.29 | 66.65 | 50.12 | 闭源 |
| - | Claude2 | Authropic | 60.57 | 98.15 | 71.84 | 66.67 | 30.21 | 闭源 |
| 🏅️ | ChatGLM2-Pro | 清华&智谱AI | 54.31 | 79.63 | 48.73 | 55.56 | 67.71 | 闭源 |
| 🥈 | SenseChat 3.0 | 商汤科技 | 54.29 | 88.89 | 56.65 | 69.7 | 43.75 | 闭源 |
| 🥉 | 文心一言(v2.3.1) | 百度 | 53.72 | 87.96 | 56.33 | 56.94 | 36.96 | 闭源 |
| 4 | Baichuan2-13B-Chat | 百川智能 | 52.45 | 86.11 | 43.04 | 44.43 | 34.38 | 开源 |
| 5 | 豆包 | 字节跳动 | 48.65 | 71.3 | 53.16 | 47.22 | 59.38 | 闭源 |
| 6 | vivoLM | vivo | 47.67 | 67.59 | 52.22 | 47.14 | 51.04 | 闭源 |
| 7 | MiniMax-Abab5.5 | MiniMax | 46.31 | 56.48 | 44.3 | 54.17 | 42.71 | 闭源 |
| 8 | Baichuan2-7B-Chat | 百川智能 | 42.28 | 67.59 | 34.81 | 36.11 | 35.42 | 开源 |
| 9 | 讯飞星火(v4.0) | 科大讯飞 | 40.64 | 47.22 | 43.99 | 37.42 | 54.17 | 闭源 |
| 10 | 通义千问(v1.0.7) | 阿里巴巴 | 33.78 | 45.37 | 37.34 | 41.67 | 13.54 | 闭源 |
| 11 | Chinese-Alpaca-2-13B | yiming cui | 32.64 | 77.78 | 22.78 | 22.21 | 43.75 | 开源 |
| 12 | OpenBuddy-Llama2-70B | OpenBuddy | 30.84 | 52.78 | 40.19 | 26.37 | 31.25 | 开源 |
| - | Llama-2-13B-Chat | Meta | 29.83 | 55.56 | 21.84 | 25.12 | 44.68 | 开源 |
| 13 | ChatGLM2-6B | 清华&智谱AI | 25.49 | 50.93 | 26.27 | 26.39 | 40.62 | 开源 |
| 14 | ERNIE-3.5-Turbo | 百度 | 24.81 | 35.19 | 21.2 | 37.5 | 51.01 | 闭源 |
| 15 | Qwen-7B-Chat | 阿里巴巴 | 23.59 | 50 | 21.2 | 27.14 | 21.88 | 开源 |
| 16 | 360GPT_S2_V94 | 360|18.97 |35.19 |16.77 |24.98 | 32.29| 闭源|

OPEN分数计算方法：与代表性领先模型（如3.5）对战后，根据胜、和和败的计算出得分，胜利得3分，和得1分，负不得分。

计算公式 =（胜利次数 * 3分 + 和次数 * 1分）/ (2分 * 对战次数)，且满分上限为100分。


### SuperCLUE-OPT三大能力客观题排行榜（2023年9月）

| 排名 | 模型 | 机构 | OPT分数 | 基础能力 | 中文特性 | 学术与专业能力 |  
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |  
| - | GPT4 | OpenAI | 81.58 | 88.13 | 80.09 | 75.35 | 
| 🏅️ | 文心一言(v2.3.1) | 百度 | 75.93 | 82.64 | 83.2 | 58.11 | 
| 🥈 | SenseChat 3.0 | 商汤科技 | 75.45 | 82.3 | 80.04 | 61.71 | 
| 🥉 | vivoLM | vivo | 74.21 | 79.27 | 81.22 | 59.2 | 
| 4 | ChatGLM2-Pro | 清华&智谱AI | 73.84 | 79.68 | 80.94 | 57.71 |  
| 5 | MiniMax-Abab5.5 | MiniMax | 73.48 | 79.31 | 80.76 | 57.14 |  
| 6 | 通义千问(v1.0.7) | 阿里巴巴 | 72 | 78.17 | 78.75 | 54.65 |  
| 7 | 豆包 | 字节跳动 | 69.86 | 78.21 | 77.44 | 49.88 |  
| 8 | gpt-3.5-turbo | OpenAI | 66.61 | 74.65 | 69.24 | 53.43 | 
| - | Claude2 | Authropic | 66.6 | 75 | 66.67 | 56.23 | 
| 9 | Baichuan2-13B-Chat | 百川智能 | 66.4 | 71.61 | 75.14 | 49.02 | 
| 10 | Qwen-7B-Chat | 阿里巴巴 | 64.97 | 72.17 | 73.61 | 45.12 | 
| 11 | OpenBuddy-Llama2-70B | OpenBuddy | 64.46 | 75.34 | 65.79 | 49.71 | 
| 13 | 360GPT_S2_V94 | 360 | 64.32 | 69.8 | 73.52 | 44.81 | 
| 12 | 讯飞星火(v4.0) | 科大讯飞 | 64.2 | 73.24 | 69.37 | 45.73 |  
| 14 | Baichuan2-7B-Chat | 百川智能 | 61.86 | 65.91 | 71.73 | 44.41 | 
| 15 | ChatGLM2-6B | 清华&智谱AI | 57.8 | 66.95 | 62.73 | 40.37 |  
| 16 | ERNIE-3.5-Turbo | 百度 | 57.19 | 63.74 | 65.76 | 38.69 | 
| 17 | Chinese-Alpaca-2-13B | yiming cui | 50.56 | 56.4 | 54.08 | 38.97 | 
| - | Llama-2-13B-Chat | Meta | 34.33 | 41.81 | 30.13 | 30.11 | 

OPT分数，根据题目的得分汇总而来（每个题目的得分/总题目数）；每一个题目属于三大能力之前，每个能力下面至少有10项子任务

### SuperCLUE十大基础能力排行榜（2023年9月）

| 模型名称 | 机构 | 计算 | 逻辑<br/>推理 | 代码 | 知识<br/>百科 | 语言理解<br/> | 对话 | 生成<br/>创作 | 角色扮演 |AI Agent | 安全 |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| GPT4 | OpenAI | 71.88 | 96.25 | 100 | 100 | 100 | 43.75 | 73.61 | 41.67 | 91.67 | 81.25 |
| ChatGLM2-Pro | 清华&智谱AI | 45.87 | 47.5 | 33.75 | 75 | 79.63 | 51.25 | 37.5 | 38.89 | 55.56 | 67.71 |
| 豆包 | 字节跳动 | 45.83 | 78.75 | 48.75 | 36.67 | 71.3 | 28.75 | 20.83 | 30.56 | 47.22 | 59.38 |
| 讯飞星火(v4.0) | 科大讯飞 | 45.76 | 47.5 | 56.25 | 20 | 47.22 | 21.25 | 38.89 | 22.22 | 37.42 | 54.17 |
| vivoLM | vivo | 40.62 | 45 | 71.25 | 55 | 67.59 | 31.25 | 31.94 | 27.78 | 47.14 | 51.04 |
| ERNIE-3.5-Turbo | 百度 | 12.5 | 36.25 | 23.75 | 11.67 | 35.19 | 11.25 | 11.11 | 4.17 | 37.5 | 51.01 |
| gpt-3.5-turbo | OpenAI | 52.08 | 70 | 62.5 | 73.33 | 72.22 | 51.25 | 69.44 | 51.39 | 66.67 | 50.12 |
| Llama-2-13B-Chat | Meta | 16.67 | 21.25 | 25 | 26.67 | 55.56 | 20 | 23.61 | 26.39 | 25.12 | 44.68 |
| SenseChat 3.0 | 商汤科技 | 41.65 | 72.5 | 67.5 | 45 | 88.89 | 33.75 | 30.56 | 25 | 69.7 | 43.75 |
| Chinese-Alpaca-2-13B | yiming cui | 9.38 | 35 | 23.75 | 26.67 | 77.78 | 20 | 36.11 | 12.5 | 22.21 | 43.75 |
| MiniMax-Abab5.5 | MiniMax | 32.29 | 62.5 | 51.25 | 66.67 | 56.48 | 27.5 | 50 | 23.61 | 54.17 | 42.71 |
| ChatGLM2-6B | 清华&智谱AI | 33.31 | 42.5 | 6.25 | 20 | 50.93 | 7.5 | 4.17 | 4.17 | 26.39 | 40.62 |
| 文心一言(v2.3.1) | 百度 | 45.91 | 52.5 | 75 | 53.33 | 87.96 | 30 | 48.61 | 36.11 | 56.94 | 36.96 |
| Baichuan2-7B-Chat | 百川智能 | 29.17 | 33.75 | 32.5 | 48.33 | 67.59 | 61.25 | 37.5 | 36.11 | 36.11 | 35.42 |
| Baichuan2-13B-Chat | 百川智能 | 19.79 | 37.5 | 61.25 | 63.33 | 86.11 | 57.5 | 68.06 | 54.17 | 44.43 | 34.38 |
| 360GPT_S2_V94 | 360 | 8.33 | 36.25 | 11.25 | 11.67 | 35.19 | 5 | 8.33 | 5.56 | 24.98 | 32.29 |
| OpenBuddy-Llama2-70B | OpenBuddy | 36.46 | 41.25 | 53.75 | 26.67 | 52.78 | 16.25 | 4.17 | 2.78 | 26.37 | 31.25 |
| Claude2 | Authropic | 73.96 | 77.5 | 62.5 | 73.33 | 98.15 | 58.75 | 34.72 | 15.28 | 66.67 | 30.21 |
| Qwen-7B-Chat | 阿里巴巴 | 14.58 | 32.5 | 18.75 | 20 | 50 | 12.5 | 19.44 | 9.72 | 27.14 | 21.88 |
| 通义千问(v1.0.7) | 阿里巴巴 | 41.61 | 35 | 26.25 | 48.33 | 45.37 | 15 | 43.06 | 30.56 | 41.67 | 13.54 |

AI Agent: AI Agent智能体能力，包括工具使用、任务规划； 语言理解，包括语言理解与抽取

### SuperCLUE开源模型排行榜（2023年9月）
| 排名 | 模型 | 机构 | 总分 | OPEN<br/>多轮开放问题 | OPT<br/>三大能力客观题 | 许可 |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| - | GPT4 | OpenAI | 83.2 | 84.28 | 81.58 | 闭源 |
| - | gpt-3.5-turbo | OpenAI | 63.74 | 61.82 | 66.61 | 闭源 |
| - | Claude2 | Authropic | 62.98 | 60.57 | 66.6 | 闭源 |
| 🏅️ | Baichuan2-13B-Chat | 百川智能 | 58.03 | 52.45 | 66.4 | 开源 |
| 🥈 | Baichuan2-7B-Chat | 百川智能 | 50.11 | 42.28 | 61.86 | 开源 |
| 🥉 | OpenBuddy-Llama2-70B | OpenBuddy | 44.29 | 30.84 | 64.46 | 开源 |
| 4 | Qwen-7B-Chat | 阿里巴巴 | 40.14 | 23.59 | 64.97 | 开源 |
| 5 | Chinese-Alpaca-2-13B | yiming cui | 39.81 | 32.64 | 50.56 | 开源 |
| 6 | ChatGLM2-6B | 清华&智谱AI | 38.41 | 25.49 | 57.8 | 开源 |
| - | Llama-2-13B-Chat | Meta | 31.63 | 29.83 | 34.33 | 开源 |

------------------------------------------------------------------------------------------------------------------------
#### 四大维度上的成绩（语言理解与生成排行榜、专业技能与知识、AI Agent-智能体、大模型安全性）：

### SuperCLUE语言理解与生成排行榜（2023年9月）
| 排名 | 模型名称 | 总分 | 语言理解与抽取 | 生成与创作 | 上下文对话 | 角色扮演 |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| - | GPT4 | 77.11 | 100 | 73.61 | 43.75 | 41.67 |
| 🏅️ | Baichuan2-13B-Chat | 68.37 | 86.11 | 68.06 | 57.5 | 54.17 |
| - | gpt-3.5-turbo | 62.05 | 72.22 | 69.44 | 51.25 | 51.39 |
| - | Claude2 | 56.93 | 98.15 | 34.72 | 58.75 | 15.28 |
| 🥈 | ChatGLM2-Pro | 54.82 | 79.63 | 37.5 | 51.25 | 38.89 |
| 🥉 | 文心一言(v2.3.1) | 54.22 | 87.96 | 48.61 | 30 | 36.11 |
| 4 | Baichuan2-7B-Chat | 52.71 | 67.59 | 37.5 | 61.25 | 36.11 |
| 5 | SenseChat 3.0 | 49.1 | 88.89 | 30.56 | 33.75 | 25 |
| 6 | vivoLM | 42.47 | 67.59 | 31.94 | 31.25 | 27.78 |
| 7 | 豆包 | 41.27 | 71.3 | 20.83 | 28.75 | 30.56 |
| 8 | MiniMax-Abab5.5 | 40.96 | 56.48 | 50 | 27.5 | 23.61 |
| 9 | Chinese-Alpaca-2-13B | 40.66 | 77.78 | 36.11 | 20 | 12.5 |
| 10 | 通义千问(v1.0.7) | 34.34 | 45.37 | 43.06 | 15 | 30.56 |
| - | Llama-2-13B-Chat | 33.73 | 55.56 | 23.61 | 20 | 26.39 |
| 11 | 讯飞星火(v4.0) | 33.73 | 47.22 | 38.89 | 21.25 | 22.22 |
| 12 | Qwen-7B-Chat | 25.6 | 50 | 19.44 | 12.5 | 9.72 |
| 13 | OpenBuddy-Llama2-70B | 22.59 | 52.78 | 4.17 | 16.25 | 2.78 |
| 14 | ChatGLM2-6B | 20.18 | 50.93 | 4.17 | 7.5 | 4.17 |
| 15 | ERNIE-3.5-Turbo | 17.47 | 35.19 | 11.11 | 11.25 | 4.17 |
| 16 | 360GPT_S2_V94 | 15.66 | 35.19 | 8.33 | 5 | 5.56 |


### SuperCLUE专业技能与知识排行榜（2023年9月）

| 排名 | 模型名称 | 总分 | 计算 | 逻辑与推理 | 代码 | 知识与百科 |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| - | Claude2 | 71.84 | 73.96 | 77.5 | 62.5 | 73.33 |
| - | GPT4 | 90.51 | 71.88 | 96.25 | 100 | 100 |
| - | gpt-3.5-turbo | 63.29 | 52.08 | 70 | 62.5 | 73.33 |
| 🥈 | 文心一言(v2.3.1) | 56.33 | 45.91 | 52.5 | 75 | 53.33 |
| 🥉 | 豆包 | 53.16 | 45.87 | 78.75 | 48.75 | 36.67 |
| 5 | ChatGLM2-Pro | 48.73 | 45.83 | 47.5 | 33.75 | 75 |
| 7 | 讯飞星火(v4.0) | 43.99 | 45.76 | 47.5 | 56.25 | 20 |
| 🏅️ | SenseChat 3.0 | 56.65 | 41.65 | 72.5 | 67.5 | 45 |
| 10 | 通义千问(v1.0.7) | 37.34 | 41.61 | 35 | 26.25 | 48.33 |
| 4 | vivoLM | 52.22 | 40.62 | 45 | 71.25 | 55 |
| 9 | OpenBuddy-Llama2-70B | 40.19 | 36.46 | 41.25 | 53.75 | 26.67 |
| 12 | ChatGLM2-6B | 26.27 | 33.31 | 42.5 | 6.25 | 20 |
| 6 | MiniMax-Abab5.5 | 44.3 | 32.29 | 62.5 | 51.25 | 66.67 |
| 11 | Baichuan2-7B-Chat | 34.81 | 29.17 | 33.75 | 32.5 | 48.33 |
| 8 | Baichuan2-13B-Chat | 43.04 | 19.79 | 37.5 | 61.25 | 63.33 |
| - | Llama-2-13B-Chat | 21.84 | 16.67 | 21.25 | 25 | 26.67 |
| 15 | Qwen-7B-Chat | 21.2 | 14.58 | 32.5 | 18.75 | 20 |
| 14 | ERNIE-3.5-Turbo | 21.2 | 12.5 | 36.25 | 23.75 | 11.67 |
| 13 | Chinese-Alpaca-2-13B | 22.78 | 9.38 | 35 | 23.75 | 26.67 |
| 16 | 360GPT_S2_V94 | 16.77 | 8.33 | 36.25 | 11.25 | 11.67 |

### SuperCLUE-Agent智能体能力排行榜（2023年9月）

| 排名 | 模型名称 | 总分 | 工具使用 | 任务规划 |
| :---: | :----: | :---: | :---: | :---: |
| - | GPT4 | 91.67 | 94.44 | 88.89 |
| 🏅️ | SenseChat 3.0 | 69.7 | 46.67 | 87.72 |
| - | Claude2 | 66.67 | 63.89 | 69.44 |
| - | gpt-3.5-turbo | 66.65 | 63.83 | 69.12 |
| 🥈 | 文心一言(v2.3.1) | 56.94 | 44.12 | 69.44 |
| 🥉 | ChatGLM2-Pro | 55.56 | 66.43 | 44.41 |
| 4 | MiniMax-Abab5.5 | 54.17 | 58.31 | 50.23 |
| 5 | 豆包 | 47.22 | 52.78 | 41.67 |
| 6 | vivoLM | 47.14 | 50.24 | 44.43 |
| 7 | Baichuan2-13B-Chat | 44.43 | 63.89 | 25.01 |
| 8 | 通义千问(v1.0.7) | 41.67 | 52.78 | 30.56 |
| 9 | ERNIE-3.5-Turbo | 37.5 | 44.34 | 30.51 |
| 10 | 讯飞星火(v4.0) | 37.42 | 44.24 | 30.43 |
| 11 | Baichuan2-7B-Chat | 36.11 | 41.67 | 30.56 |
| 12 | Qwen-7B-Chat | 27.14 | 17.65 | 36.01 |
| 13 | ChatGLM2-6B | 26.39 | 27.78 | 25 |
| 14 | OpenBuddy-Llama2-70B | 26.37 | 22.21 | 30.56 |
| - | Llama-2-13B-Chat | 25.12 | 38.89 | 11.11 |
| 15 | 360GPT_S2_V94 | 24.98 | 19.43 | 30.56 |
| 16 | Chinese-Alpaca-2-13B | 22.21 | 19.42 | 25.13 |

### SuperCLUE安全性排行榜（2023年9月）

| 排名 | 模型 | 总分 | 传统安全 | 指令攻击 |
| :---: | :---: | :---: | :---: | :---: |
| - | GPT4 | 81.25 | 83.93 | 77.51 |
| 🏅️ | ChatGLM2-Pro | 67.71 | 67.86 | 67.53 |
| 🥈 | 豆包 | 59.38 | 64.29 | 52.45 |
| 🥉 | 讯飞星火(v4.0) | 54.17 | 55.36 | 52.49 |
| 4 | vivoLM | 51.04 | 58.93 | 40.12 |
| 5 | ERNIE-3.5-Turbo | 51.01 | 50 | 52.51 |
| - | gpt-3.5-turbo | 50.12 | 39.29 | 65.12 |
| - | Llama-2-13B-Chat | 44.68 | 46.43 | 42.11 |
| 6 | SenseChat 3.0 | 43.75 | 50.21 | 35.12 |
| 7 | Chinese-Alpaca-2-13B | 43.75 | 35.71 | 55.24 |
| 8 | MiniMax-Abab5.5 | 42.71 | 37.5 | 52.63 |
| 9 | ChatGLM2-6B | 40.62 | 33.93 | 50.12 |
| 10 | 文心一言(v2.3.1) | 36.96 | 28.85 | 47.51 |
| 11 | Baichuan2-7B-Chat | 35.42 | 35.71 | 35.12 |
| 12 | Baichuan2-13B-Chat | 34.38 | 32.14 | 37.51 |
| 13 | 360GPT_S2_V94 | 32.29 | 16.07 | 55.23 |
| 14 | OpenBuddy-Llama2-70B | 31.25 | 26.79 | 37.56 |
| - | Claude2 | 30.21 | 39.29 | 17.57 |
| 15 | Qwen-7B-Chat | 21.88 | 16.07 | 30.01 |
| 16 | 通义千问(v1.0.7) | 13.54 | 3.57 | 27.59 |


### 9月测评改进

#### 1. 模型变动
1）新增商汤商量SenseChat 3.0大模型、vivo的vivoLM大模型、字节跳动的豆包大模型。
 
2）本次评测了百度的两个版本模型，分别为网页版文心一言(v2.3.1)与API版本ERNIE-3.5-Turbo。（注：过去8月份OPT选择题评测的是ERNIE-3.5-Turbo的API，OPEN开放问题评测的是文心一言的网页版）。

3）ChatGLM闭源模型由ChatGLM-130B升级为ChatGLM2-Pro。

具体被测模型的配置信息见Github的ModelCard。Github地址：https://github.com/CLUEbenchmark/SuperCLUE

#### 2. 评测任务变动
本月评测任务新增AI智能体，重点评估AI Agent在【工具使用】和【任务规划】两个关键能力上的表现。

#### 3. 评分机制变动
SuperCLUE结合大模型市场技术进展及国内外评测基准现状，对综合性评测总分评分逻辑进行优化。

1）多轮开放评测OPEN评分标准：在与基线模型对战过程中，我们认为胜的情况价值意义更大。所以，本次OPEN测评将胜（1分）调整为胜（3分）。如一道题目对战，胜得3分，平局得1分，负得0分。

2）我们发现客观选择题并不能考察中文大模型的真实综合能力，多轮主观题的能力尤为重要，所以我们在计算总分时，将OPEN的权重由50%提升至60%。


### 示例
#### 能力1：语义理解与抽取

这是一种语言能力，能够理解并解析输入的文字信息的含义。模型需要能够识别短语、句子、段落的含义，同时还要能从更大的文本块中抽取关键信息和主题。

##### 多轮对话示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_nlp.png"  width="100%" height="100%"></img>

注：本示例中可同时评测多轮对话能力

#### 能力2：AI agent（智能体）能力

AI agent（智能体）是当前与大语言模型相关的前沿研究热点，拥有类似贾维斯等科幻电影中人类超级助手的能力，可以根据需求自主的完成任务。

重点评估AI agent在【工具使用】和【任务规划】两个关键能力上的表现

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_agent.png"  width="100%" height="100%"></img>


#### 能力3：上下文对话

这是一种语言能力，需要理解并记住前面的对话信息，以便在回答中保持连贯性。这涉及到理解对话的整体流程和上下文环境，或生成相应的对话。

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_dial.png"  width="100%" height="100%"></img>

#### 能力4：生成与创作

这是一种语言能力，能够创造新的文本内容，如文章、文案、短故事、诗歌。这涉及到创造性地运用语言，同时还要考虑到风格、语境和目标读者。

##### 示例
<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_generate.png"  width="100%" height="100%"></img>


#### 能力5：知识与百科

这是一种知识能力，能够像百科全书一样提供知识信息。这涉及到理解和回答关于广泛主题的问题，以及提供准确、详细和最新的信息。

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_knowledge.png"  width="100%" height="100%"></img>


#### 能力6：代码

这是一种专业能力，能够理解和生成编程代码。这涉及到理解多种编程语言的语法、结构和习惯，以及如何解决编程问题。

##### 多轮对话示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_code.png"  width="100%" height="100%"></img>

注：本示例中可同时评测多轮对话能力

#### 能力7：逻辑与推理

这是一种专业能力，能够理解和应用逻辑原则进行推理。这涉及到分析问题、识别问题及推理。

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_logic.png"  width="100%" height="100%"></img>


####  能力8：计算

这是一种专业能力，使其能够执行数学运算，如加法、减法、乘法和除法，甚至更复杂的数学问题。这涉及到理解数学问题的表述，以及如何步骤地解决这些问题。

##### 多轮对话示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_compute.png"  width="100%" height="100%"></img>

注：本示例中可同时评测多轮对话能力

####  能力9：角色扮演

这是一种感知能力，使其能够在特定的模拟环境或情景中扮演一个角色。这涉及到理解特定角色的行为、说话风格，以及在特定情境下的适当反应。

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_roleplay.png"  width="100%" height="100%"></img>


####   能力10：安全

这是一种安全能力，防止生成可能引起困扰或伤害的内容。这涉及到识别和避免可能包含敏感或不适当内容的请求，以及遵守用户的隐私和安全政策。

##### 示例

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/r2309/image_safety.png"  width="100%" height="100%"></img>

### 8月榜单更新情况
1.综合性：将OPEN多轮开放问题与OPT三大能力客观题进行了结合起来，作为8月榜单；

2.模型细节：Baichuan-13B-Chat使用了是最新的模型权重，具体见huggingface的权重；文心一言，OPT三大能力客观题使用的是API（Ernie-3.5-turbo）；
  360使用的是api版本；

3.模型更新：去除了一些前期大家比较关注但当前活跃度不高的模型，如MOSS，BELLE等；加入了一些如Qwen-7B-Chat和3个Llam2相关模型。
