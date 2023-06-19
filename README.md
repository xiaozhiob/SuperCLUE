# SuperCLUE
中文通用大模型综合性基准SuperCLUE

SuperCLUE: A Benchmark for Foundation Models in Chinese


- [SuperCLUE是什么](#SuperCLUE是什么)
- [SuperCLUE的构成与特点](#SuperCLUE的构成与特点)
- [SuperCLUE的测试结果](#SuperCLUE的测试结果)
     - [总榜单](#2023年6月Superclue中文大模型总排行榜)
     - [基础能力表](#2023年6月SuperCLUE基础能力榜单)
     - [中文特性能力表](#2023年6月SuperCLUE中文特性榜单)
- [SuperCLUE的特点](#SuperCLUE的特点)
- [SuperCLUE的数据集](#SuperCLUE的数据集)
- [人类基准测评](#人类基准测评)
- [实验分析](#实验分析)
     - [人类与模型的对比](#人类与模型的对比)
     - [模型层面-宏观分析](#模型层面-宏观分析)
     - [能力角度分析](#能力角度分析) 
     - [国内大模型点评](#国内大模型点评) 
- [SuperCLUE的不足与局限](#SuperCLUE的不足与局限)
- [SuperCLUE的常见问答](#SuperCLUE的常见问答)
- [SuperCLUE讨论与交流](#SuperCLUE讨论与交流)

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/superclue.jpeg"  width="90%" height="90%"></img>

SuperCLUE基准计划按照月度进行更新，纳入更多可用中文大模型，欢迎联系与交流；数据集和进一步信息计划在下一次更新时公开，敬请期待。
##### 新增2023-5-31
<a href='https://www.SuperCLUEAI.com'>中文通用大模型匿名对战评价基准，SuperCLUE琅琊榜</a>

##### 更新 
    更新 Update（2023-06-19）
    SuperCLUE中文大模型排行榜(2023年6月) 
    
    更新 Update（2023-05-30）
    添加RWKV-7B,IDEA-姜子牙-13B,西湖大模型v2       
    
    更新 Update（2023-05-21）
    添加360智脑
    
    更新 Update（2023-05-12）
    添加Claude: OpenAI最强竞争对手Anthropic的Claude取得了与ChatGPT3.5一致的效果
    添加ChatGLM-130B: 相比ChatGLM-6B效果大幅提升（+7.35），处于国内较好水平

## SuperCLUE是什么
中文通用大模型基准（SuperCLUE），是针对中文可用的通用大模型的一个测评基准。

它主要回答的问题是：在当前通用大模型大力发展的背景下，中文大模型的效果情况，包括但不限于"这些模型不同任务的效果情况"、"相较于国际上的代表性模型做到了什么程度"、
"这些模型与人类的效果对比如何"。

它尝试在一系列国内外代表性的模型上使用多个维度能力进行测试。SuperCLUE是中文语言理解测评基准（CLUE）在通用人工智能时代的进一步发展。

<img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/superclue_202306.jpeg"  width="100%" height="100%"></img>


## SuperCLUE的测试结果
四个表格：汇总表、基础能力表、专业能力表、中文特性能力表

#####  排行榜会定期更新           数据来源: www.CLUEbenchmarks.com              

### 2023年6月SuperCLUE中文大模型总排行榜

| 排名 | 模型 | 机构 | 平均 | 基础能力 | 中文特性 | 学术专业 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 🧝 | 人类 | CLUE | 93.09 | 92.11 | 94.06 | -- |
| 🏅 | <a href='https://openai.com/'>GPT-4</a>| OpenAI | 78.76 | 82.13 | 83.81 | 70.35 |
| 🥈 | <a href='https://openai.com/'>gpt-3.5-turbo</a> | OpenAI | 67.98 | 75.44 | 74.14 | 54.37 |
| 🥉 | <a href='https://ai.360.cn'>360智脑(4.0)</a>| 360 | 63.53 | 71.68 | 73.04 | 45.87 |
| 4 | <a href='https://yiyan.baidu.com/welcome'>文心一言(v2.0.4)</a> | 百度 | 62.85 | 70.64 | 71.72 | 46.18 |
| 5 | <a href='https://www.anthropic.com/'>Claude-instant </a> | Authropic | 60.38 | 68.74 | 60.73 | 51.67 |
| 6 | <a href='https://xinghuo.xfyun.cn/'>讯飞星火(v1.5)</a> | 科大讯飞 | 59.80 | 69.92 | 67.18 | 42.29 |
| 7 | <a href='https://api.minimax.chat/'>MiniMax-abab5</a>| MiniMax | 58.19 | 63.15 | 69.38 | 42.05 |
| 8 | <a href='https://chatglm.cn'>ChatGLM-130B</a> | 清华大学&智谱AI | 51.53 | 53.62 | 64.25 | 36.73 |
| 9 | <a href='https://github.com/LianjiaTech/BELLE'>BELLE-13B</a> | 链家 | 50.65 | 60.68 | 52.97 | 38.31 |
| 10 | <a href='https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1'>IDEA-姜子牙-13B</a>|深圳IDEA研究院| 48.67 | 59.12 | 51.36 | 35.53 |
| 11 | <a href='https://github.com/THUDM/ChatGLM-6B'>ChatGLM-6B</a> | 清华大学&智谱AI | 48.56 | 54.69 | 56.26 | 34.74 |
| 12 | <a href='https://github.com/baichuan-inc/baichuan-7B'>baichuan-7B</a> | 百川智能 | 48.18 | 54.06 | 55.16 | 35.32 |
| 13 | <a href='https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b'>phoenix-7B</a> | 香港中文大学 | 43.60 | 50.97 | 46.29 | 33.55 |
| 14 | <a href='https://github.com/OpenLMLab/MOSS'>MOSS-16B</a> | 复旦大学 | 38.56 | 44.64 | 40.37 | 30.68 |
| 15 | <a href='https://github.com/lm-sys/FastChat'>Vicuna-13B</a> | UC伯克利 | 29.15 | 36.74 | 27.17 | 23.54 |
| 16 | <a href='https://github.com/BlinkDL/ChatRWKV'>RWKV-Raven-7B</a> | RWKV基金会 | 24.83 | 26.21 | 23.66 | 24.60 |
| 17 | <a href='https://model.baai.ac.cn/model-detail/100098'>Aquila-7B</a> | 智源研究院 | 23.71 | 22.55 | 25.84 | 22.73 |


### 2023年6月SuperCLUE基础能力榜单


| 排名 | 模型 | 平均分 | 语义理解 | 闲聊 | 上下文对话 | 角色扮演 | 百科与知识 | 生成与创作 | 代码 | 逻辑与推理 | 计算 | 安全 |
|:---:|:-----:|:-----:|:-------:|:---:|:-------:|:-----:|:-------:|:-------:|:---:|:-------:|:---:|:---:|
| 🧝 | 人类 | 	92.11 | 	90.91 | 	95.37 | 	91.28 | 	92.44 | 	97.81 | 	86.27 | 	86.28 | 	90.24 | 	95.82	|  94.69 | 
| 🏅 | GPT-4 | 82.13 | 92.93 | 93.00 | 86.36 | 84.83 | 92.11 | 79.41 | 71.84 | 68.09 | 60.00 | 90.35 |
| 🥈 | gpt-3.5-turbo | 75.44 | 87.88 | 92.00 | 80.91 | 86.90 | 92.98 | 75.49 | 62.14 | 41.49 | 37.27 | 89.47 |
| 🥉 | 360智脑(4.0) | 71.68 | 88.89 | 91.00 | 86.36 | 79.31 | 88.60 | 66.67 | 43.69 | 36.17 | 46.36 | 82.46 |
| 4 | 文心一言(v2.0.4) | 70.64 | 80.61 | 81.00 | 74.55 | 76.55 | 82.46 | 70.59 | 52.43 | 52.13 | 53.64 | 78.07 |
| 5 | 讯飞星火(v1.5) | 69.92 | 74.75 | 83.00 | 74.55 | 73.10 | 78.07 | 65.31 | 38.84 | 59.57 | 67.27 | 80.70 |
| 6 | Claude-instant | 68.74 | 76.77 | 87.00 | 77.27 | 77.93 | 81.58 | 64.71 | 48.54 | 42.55 | 43.64 | 80.70 |
| 7 | MiniMax-abab5 | 63.15 | 74.75 | 85.00 | 73.64 | 77.24 | 80.70 | 64.71 | 33.98 | 25.53 | 30.00 | 76.32 |
| 8 | BELLE-13B | 60.68 | 77.78 | 82.00 | 70.91 | 71.03 | 75.44 | 53.92 | 36.89 | 32.98 | 32.73 | 66.67 |
| 9 | IDEA-姜子牙-13B(v1.1) | 59.12 | 74.75 | 77.00 | 72.73 | 68.28 | 67.54 | 63.73 | 29.13 | 34.04 | 31.82 | 66.67 |
| 10 | ChatGLM-6B | 54.69 | 71.72 | 73.20 | 55.45 | 73.79 | 64.91 | 53.92 | 25.24 | 30.85 | 22.73 | 66.67 |
| 11 | baichuan-7B | 54.06 | 71.43 | 71.00 | 63.64 | 61.97 | 57.52 | 46.88 | 34.21 | 34.78 | 28.30 | 60.53 |
| 12 | ChatGLM-130B | 53.62 | 35.35 | 75.00 | 78.18 | 73.79 | 77.19 | 62.75 | 33.01 | 30.85 | 26.36 | 33.33 |
| 13 | phoenix-7B | 50.97 | 70.71 | 68.00 | 54.55 | 60.69 | 63.16 | 42.16 | 35.64 | 23.40 | 25.93 | 58.77 |
| 14 | MOSS-16B | 44.64 | 67.68 | 56.00 | 46.36 | 56.55 | 38.60 | 55.88 | 26.21 | 31.91 | 21.82 | 42.98 |
| 15 | Vicuna-13B | 36.74 | 35.42 | 43.00 | 40.91 | 45.52 | 24.56 | 30.39 | 38.61 | 38.30 | 32.73 | 35.96 |
| 16 | RWKV-Raven-7B | 26.21 | 20.20 | 29.00 | 17.27 | 28.97 | 24.56 | 24.51 | 31.07 | 30.85 | 26.36 | 28.95 |
| 17 | Aquila-7B | 22.55 | 27.27 | 24.00 | 22.73 | 22.07 | 28.07 | 22.55 | 19.42 | 17.02 | 15.45 | 26.32 |

  
     指标为：Accuracy。数据表比较大，表格请往后拉        

### 2023年6月SuperCLUE中文特性榜单

| 排名 | 模型 | 平均分 | 字形和拼音 | 字义理解 | 句法分析 | 文学 | 诗词 | 成语 | 歇后语和谚语 | 方言 | 对联 | 古文 |
|:---:|:-----:|:-----:|:-------:|:---:|:-------:|:-----:|:-------:|:-------:|:---:|:-------:|:---:|:---:|
| 🧝	|人类	|94.06	|97.89|	94.27	|90.42|	94.28|	95.62|	97.26|	93.02|	92.80|	94.65	|90.35|
| 🏅️ | GPT-4 | 83.81 | 76.87 | 81.31 | 87.10 | 87.41 | 79.86 | 95.95 | 91.43 | 73.85 | 84.29 | 78.87 |
| 🥈 | gpt-3.5-turbo | 74.14 | 64.63 | 71.03 | 75.81 | 82.52 | 69.44 | 90.54 | 80.00 | 58.46 | 80.71 | 66.20 |
| 🥉 | 360智脑 | 73.04 | 46.94 | 73.83 | 66.94 | 88.81 | 75.00 | 93.92 | 84.29 | 52.31 | 77.14 | 69.01 |
| 4 | 文心一言 | 71.72 | 58.50 | 73.83 | 62.90 | 70.63 | 75.00 | 86.49 | 85.00 | 70.00 | 68.57 | 65.49 |
| 5 | MiniMax-abab5 | 69.38 | 44.90 | 73.83 | 66.13 | 81.82 | 72.92 | 89.19 | 85.00 | 56.15 | 56.43 | 66.90 |
| 6 | 讯飞星火 | 67.18 | 50.34 | 73.83 | 66.13 | 74.13 | 54.17 | 86.49 | 85.00 | 50.00 | 70.71 | 61.27 |
| 7 | ChatGLM-130B | 64.25 | 48.30 | 27.10 | 58.87 | 79.72 | 72.22 | 85.14 | 83.57 | 43.08 | 69.29 | 63.38 |
| 8 | Claude-instant  | 60.73 | 44.22 | 68.22 | 67.74 | 60.84 | 52.08 | 79.73 | 72.86 | 46.92 | 58.57 | 57.75 |
| 9 | ChatGLM-6B | 56.26 | 33.33 | 57.01 | 48.39 | 59.44 | 56.25 | 78.38 | 70.00 | 36.92 | 66.43 | 54.23 |
| 10 | baichuan-7B | 55.16 | 31.29 | 57.01 | 55.56 | 62.24 | 56.94 | 81.08 | 73.57 | 30.77 | 52.14 | 49.30 |
| 11 | BELLE-13B | 52.97 | 40.82 | 56.07 | 62.10 | 59.44 | 50.00 | 65.54 | 62.86 | 30.00 | 58.57 | 44.37 |
| 12 | IDEA-姜子牙-13B | 51.36 | 33.33 | 56.07 | 54.03 | 53.85 | 54.17 | 73.65 | 60.71 | 26.92 | 54.29 | 45.77 |
| 13 | phoenix-7B | 46.29 | 30.61 | 61.68 | 37.90 | 56.64 | 44.44 | 67.81 | 51.43 | 26.15 | 43.57 | 43.66 |
| 14 | MOSS-16B | 40.37 | 33.33 | 50.47 | 30.65 | 45.45 | 28.47 | 58.11 | 39.29 | 26.92 | 43.57 | 47.18 |
| 15 | Vicuna-13B | 27.17 | 26.53 | 33.64 | 29.03 | 18.88 | 21.53 | 22.76 | 29.29 | 23.08 | 36.43 | 32.39 |
| 16 | Aquila-7B | 25.84 | 26.53 | 25.23 | 28.23 | 28.57 | 20.14 | 20.95 | 33.57 | 25.38 | 19.29 | 30.99 |
| 17 | RWKV-Raven-7B | 23.66 | 23.81 | 20.56 | 22.58 | 27.27 | 20.42 | 28.38 | 25.71 | 14.06 | 27.86 | 23.94 |
    
     指标为：Accuracy。数据表比较大，表格请往后啦。       
   
 #### 2023年6月SuperCLUE-70亿参数量级榜单
  
 | 排名 | 模型 | 机构 | 平均 | 基础能力 | 中文特性 | 学术专业 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 🧝 | 人类 | CLUE | 93.09 | 92.11 | 94.06 | -- |
| 🏅 | ChatGLM-6B | 清华大学&智谱AI | 48.56 | 54.69 | 56.26 | 34.74 |
| 🥈| baichuan-7B | 百川智能 | 48.18 | 54.06 | 55.16 | 35.32 |
| 🥉 | phoenix-7B | 香港中文大学 | 43.60 | 50.97 | 46.29 | 33.55 |
| 4 | RWKV-7B | RWKV基金会 | 24.83 | 26.21 | 23.66 | 24.60 |
| 5 | Aquila-7B | 智源研究院 | 23.71 | 22.55 | 25.84 | 22.73 |
  
 往期榜单，见<a href='./README_2305.md'>2023年5月SuperCLUE中文特性榜单</a>
 

### SuperCLUE的构成与特点
着眼于综合评价大模型的能力，使其能全面地测试大模型的效果，又能考察模型在中文特有任务上的理解和积累。我们对能力进行了划分，
SuperCLUE从三个不同的维度评价模型的能力：基础能力、专业能力和中文特性能力。

#### 基础能力:

包括了常见的有代表性的模型能力，如语义理解、对话、逻辑推理、角色模拟、代码、生成与创作等10项能力。

#### 专业能力:

包括了中学、大学与专业考试，涵盖了从数学、物理、地理到社会科学等50多项能力。

#### 中文特性能力:

针对有中文特点的任务，包括了中文成语、诗歌、文学、字形等10项多种能力。

#### SuperCLUE的特点：
1）多个维度能力考察（3大类，70+子能力）：从三个不同角度对中文大模型进行测试，以考察模型的综合能力；并且每一个子能力又含有十项或以上不同的细分能力。

2）自动化测评（一键测评）：通过自动化测评方式以相对客观形式测试不同模型的效果，可以一键对大模型进行测评。

3）广泛的代表性模型（17个模型）：选取了多个国内外有代表性的可用的模型进行测评，以反映国内大模型的发展现状并了解与国际领先模型的差距或相对优劣势。

4）人类基准：在通用人工智能发展的背景下，SuperCLUE也提供了模型相对于人类效果的指标对比。

### 数据集数量
    2023年6月榜单，针对基础能力、中文特性和专业能力，使用了3714题目。
    
## SuperCLUE的数据集
1.基础能力（10项能力）：语义理解、生成与创作、闲聊、对话、百科与知识、逻辑与推理、计算能力、代码、角色模拟、安全
    
    示例：
    语义理解：
        两个男人正常交谈，其中一个男人夸赞对方办事能力强，对方回答“哪里，哪里”。这里的“哪里，哪里”是什么意思？
        A. 讲话十分含糊不清。
        B. 要求说出具体的优点。
        C. 表达自己的谦虚。
        D. 挑衅对方。
         
    逻辑与推理：
        小明的妻子生了一对双胞胎。以下哪个推论是正确的？
        A. 小明家里一共有三个孩子。
        B. 小明家里一共有两个孩子。
        C. 小明家里既有男孩子也有女孩子。
        D. 无法确定小明家里孩子的具体情况。
 
     

2.中文特性能力（10项能力）：成语、诗词、文学、字义理解、汉语句法分析、汉字字形和拼音理解、歇后语和谚语、对联、方言、古文
    
    示例：
    成语：
    选出下列句子中成语使用错误的一项
        A. 这个项目时间紧任务重，大家都在马不停蹄地奔波劳碌。
        B. 他常常口是心非，让人难以相信他说的话。
        C. 两人是同学三年，一直保持着良好的关系，相互尊重、相敬如宾。
        D. 当地突发大火，整个村庄都鸡犬不宁，局势十分危急。
     
    文学：
    下列有关名著的表述有误的一项是
        A. 《红楼梦》是中国古代小说中的巅峰之作，以其瑰丽的语言和丰富的人物形象而闻名于世。
        B. 《西游记》是中国古代四大名著之一，讲述了哪吒等人历经九九八十一难，最终取得真经的故事。
        C. 《孔乙己》是鲁迅的代表作之一，以其深刻的社会洞察力和优美的文学风格而广受好评。
        D. 《围城》是钱钟书的代表作之一，以其独特的文学语言和深刻的社会洞察力而成为现代中国文学的经典之作。
         
     
3.专业能力（50+能力）：抽象代数、天文学、临床知识、大学生物学、大学计算机科学、大学数学、高中化学、高中物理、机器学习、营养、专业会计、职业心理学等
    
    示例：
    物理：
    以下物理常识题目，哪一个是错误的?
        A. 在自然环境下，声音在固体中传播速度最快。
        B. 牛顿第一定律：一个物体如果不受力作用，将保持静止或匀速直线运动的状态。
        C. 牛顿第三定律：对于每个作用力，都有一个相等而反向的反作用力。
        D. 声音在空气中的传播速度为1000m/s。
     
    天文学：
    以下天文学常识题目，哪一个是错误的？
        A. 太阳系是指由太阳和围绕着它运行的八大行星、矮行星、卫星、小行星带和彗星组成的一个行星系统。
        B. 卫星是指绕行星或其他天体运动的天体。
        C. 彗星是指太阳系中一种较小的天体，其核心由冰和尘埃组成。
        D. 按一般的天体归类方法，月球属于行星。
    
## SuperCLUE全自动测评过程：
    1、统一prompt：针对每一个题目，构造了统一的prompt供模型和人类使用；
    2、预测：系统使用模型进行预测，要求模型选取ABCD中的某一个选项；
    3、打分：如果模型的回答不是标准的答案，而是一段文字，系统会采取特定的策略自动提取出模型的答案。该策略结合模型的表现进行优化和完善。
      （注：当无法提取有效答案的时候，则表明模型没有按照人类的要求做题，未正确理解指令，则认为模型回答错误。）
       
   由于此次为SuperCLUE首次全自动测评，为了谨慎起见，全部答案事后已由多位人类进行交叉复核，与自动测评结果基本一致。

## 人类基准测评
针对于基础能力和中文特性能力题目，会有三位独立的人类测评员根据题目作答。人类测评结果，采用多数投票方式进行汇总，作为人类基准分数。

## 实验分析

#### 人类与模型的对比

从人类测评角度看，基础能力（92%）+ 中文特性能力（94%），都达到了非常高的水平。除GPT-4外，人类准确率大幅超过了其他的大模型（如在基础能力上超过其他模型15多个百分点）。
 AI虽然进展很快，但人类还是有相对优势的， 比如在计算方面，人类比最强模型GPT-4高出了30个百分点。

   
#### 模型层面-宏观分析

一句话点评：国际先进模型的效果具有较大的领先性；同时国产GPT模型也有不俗的表现，有差距但可追赶。

1）中文大模型的必要性

在国际上效果非常棒的Vicuna-13B模型，在中文领域的效果是众多模型中比较一般的模型（排名靠后）。而国内研发的大模型或在中文任务上进行训练后的模型，都大幅超过了Vicuna-13B的效果，比如星火认知大模型在总分上超过了 Vicuna-13B 20个百分点，并且BELLE-13B（基于LLaMA并在中文上训练和微调过的模型）的总分也超过了 Vicuna-13B 10多个百分点。
    
2）国内大模型与OpenAI GPT之间的差距较大，但在逐渐逼近

 可以看到在本次SuperCLUE上效果最好的国内模型，星火认知大模型，与GPT-4相比有23个百分点的差距，与gpt-3.5-turbo在总分上也有13个百分点的差距。但是我们更应该看到，
 不断涌现和迭代的国内大模型也在逐步地缩小与OpenAI GPT模型模型的差距。
 
3）gpt-3.5-turbo与GPT-4之间也有明显差距

   比如，GPT-4在所有参与测评的模型中是独一档的存在，超过了gpt-3.5-turbo近10个百分点。它在逻辑推理能力、生成与创作能力方面，远远优于其他模型（超过其他模型20个百分点或以上）。
   

#### 能力角度分析

1） 当前模型在基础能力普遍表现不错，但中文特性能力、专业能力还比较差。

   说明当前国内大模型已经有不错的基础（60-70%），但在专业领域、中文任务上表现一般（如30-60%直接），说明在专业领域或中文任务上还需要继续努力，或者说进行针对性的训练。
   
2）当前模型通常在逻辑推理、计算方面能力较差。

  除GPT-4外，其他模型在这两项能力上通常在30-50分之间。

3）角色模拟，AI模型比较擅长。
  这方面可以是非常有用的。可以让AI根据场景和角色设定帮忙人类来完成多种不同的任务，例如市场营销策划、心理咨询、客户服务、到提供创意或想法等。

#### 国内大模型点评

本次测评中，国内大模型中360智脑、讯飞星火认、文心一言、MiniMax模型有不错的表现。


## SuperCLUE的不足与局限
1. 基础能力、中文特性能力：虽然每一部分都包含了10类子能力，但这两个能力的总数据量比较少，可能存在需要扩充数据集的问题。
2. 选取模型的不完全：我们测试了9个模型，但还存在着更多的可用中文大模型。需要后续进一步添加并测试；有的模型由于没有广泛对外提供服务，我们没能获取到可用的测试版本。
3. 选取的能力范围：我们尽可能的全面、综合衡量模型的多维度能力，但是可能有一些模型能力没有在我们的考察范围内。后续也存在扩大考察范围的可能。
4. 客观考察的不足：我们以相对客观形式考察模型能力，但一些主观、开放性问题的模型能力的考察可能存在不足。
5. 模型参数：当前大模型发展较快，参数量又有比较大的差异，本次的测评并没有在同一级别的参数量上进行。

## SuperCLUE的常见问答

1. 什么时候会公布评测集和更多细节？

       由于本轮评测尚未结束，数据集和进一步信息计划将在本轮SuperCLUE评测结束后公开，敬请期待。     

2. 测试方法
       
       相同的prompt情况下，让不同的模型对题目进行预测结果，与正确答案进行匹配，计算最终结果，并统计准确率（ACC）。
       计算正确答案：根据模型预测结果，系统会提取答案，并计算题目的分数；为稳妥起见，人工会符合每一个模型的预测结果及其答案。

3. 为什么人工测评的成绩这么高? 人类测评员是什么水平？
       
       当前报告的人类测评的分数是采取开卷考试形式的进行的。即由每一个题目3个人类测评员进行开卷考试，最后结果进行多数投票后获得。
       我们也会添加采取闭卷形式的人类分数。
       
       人类测评员是高年级本科生、研究生水平。

       

## SuperCLUE讨论与交流

SuperCLUE榜单大模型评测申请：https://wj.qq.com/s2/12305633/a73d/

模型内测需求收集：https://wj.qq.com/s2/12307825/2ae0/



<p float="left">   
  <img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/superclue6group.jpeg"  width="30%" height="30%"></img>
  <img src="https://github.com/CLUEbenchmark/SuperCLUE/blob/main/resources/brightmart_s.jpeg"  width="30%" height="30%"></img>
</p> 

 
<a href="https://discord.gg/GPHv9BfNUD" target="__blank">Discord SuperCLUE交流群</a>

## 引用

如果使用本项目的，请引用本项目。

    @misc{SuperCLUE,
      author = {Liang Xu, Xuanwei Zhang, Kangkang Zhao, Lei Zhu and others from SuperCLUE team},
      title = {SuperCLUE: A Benchmark for Foundation Models in Chinese},
      year = {2023},
      publisher = {GitHub},
      journal = {GitHub repository},
      howpublished = {\url{https://github.com/CLUEbench/SuperCLUE}},
    }
