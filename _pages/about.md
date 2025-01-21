---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

大家好！我是**付弋洋**，目前本科三年级，就读于[中国人民大学](https://www.ruc.edu.cn)计算机科学与技术（图灵实验班）和金融科技实验班（高礼研究院）。

我对人工智能和金融科技充满热情，自入学以来，积极参与各类科研项目和学术竞赛，曾获得**国家奖学金**（2023-2024年）、**中国人民大学学习优秀奖学金**、**三好学生**、**优秀学生骨干奖学金**等荣誉。我的科研方向涵盖了**大语言模型的垂直领域应用**、**AI for Education**等领域。

# 🎓 Education Background
- **2022.09 - now**, 中国人民大学，北京，计算机科学与技术（图灵实验班），本科。
- **2023.02 - now**, 中国人民大学，北京，金融科技实验班（高礼研究院），本科（辅修）。
- **2023.09 - 2023.12**, UC Davis，California，Computer Science，Exchange Student。

# 📖 Basic Information

- **在校成绩：** GPA：3.84/4.0 ，**GPA 排名：1/30** 
- **语言能力：** 英语能力优异，[托福成绩为109/120](https://baiyingzhuying.github.io/docs/ENGLISHtofel.pdf)（其中：阅读29/30，听力30/30），[GRE成绩为321分](https://baiyingzhuying.github.io/docs/ENGLISHgre.pdf)。曾在加州大学戴维斯分校进行交换学习，且交换期间所有课程成绩均为满绩(A+/A)  
- **核心课程：** 高等数学 (91, 90)、高等代数 (93, 93)、数据结构与算法 (95, 93)、机器学习 (95)、数字信号处理 (95)、计算机系统基础 (90, 90)、编译原理 (92)、运筹学建模与算法 (94)  
- **编程能力：** 熟练掌握 C++、Python，熟悉算法与数据结构，抽象能力强，代码风格良好；熟练掌握 PyTorch、Numpy、Pandas，熟悉各类深度学习模型及其编程实现；具备优秀的编程/建模能力，多次获数学建模/数据挖掘比赛奖项（美赛M奖、Kaggle铜牌）  
- **开发工具：** VS Code，PyCharm，Jupyter Notebook，LaTeX (Overleaf)，Git  
- **在校荣誉：** 曾获 **国家奖学金**、中国人民大学学习优秀奖学金、中国人民大学优秀学生骨干奖学金、中国人民大学三好学生、中国人民大学优秀学生干部，在校累计获奖逾￥30000



# 🔍 Research Experience

## **💡💡💡 MAIC: 不知道叫什么名字的退课预测** <sub> &nbsp;&nbsp;[[项目主页]](https://mumuyeye.github.io/HaMonitorSentry/README.html) [[项目代码]](https://github.com/mumuyeye/HaMonitorSentry)</sub>

- **时间：** 2024.8 - 至今  
- **领域：** **LLM垂域应用、AI4Education**  
- **角色：** 共同第一作者/第一发明人  
- **研究背景：**  
- **我们的方法：**  
- **项目成果：**  
  * 相关论文已基本完成，预计投稿于 **ACL 2025**（共同第一作者）；相关专利已完成申请（第一发明人）。

---

## **💡💡💡 SOAY: A Solution-based LLM API-using Methodology for Academic Information Seeking** <sub> &nbsp;&nbsp;[[arXiv]](https://arxiv.org/abs/2405.15165) | [[Code]](https://github.com/RUCKBReasoning/SoAy) | [[Demo]](https://soay.aminer.cn/) </sub>

- **时间：** 2024.1 - 2024.8  
- **领域：** **LLM垂域应用、AI4Education**  
- **角色：** 本科生作者之一
- **研究背景：**  
  1. 日常学术活动经常需要各类学术信息，如论文的元数据、学者的出版记录以及学者之间的联系，学术信息检索系统的出现，如DBLP、Google Scholar、AMiner，大大降低了探索学术数据的复杂性。
  2. 得益于LLM理解自然语言表达意图的推理能力，学术信息寻求所需努力被进一步减少；目前，让LLM尝试去利用现有的学术检索/挖掘API越来越可行。
  3. 然而，这种尝试面临两个主要挑战：
     - (a) **耦合：** 学术查询的学术信息分布在各种存储位置，但其内部相互连接，导致多个学术API虽然负责不同的功能，但实际上却相互耦合，这种情况下，LLM需要去完全理解这些API之间调用的顺序，这是现有的API使用方法所不具备的。
     - (b) **效率：** 现有方法如ToolLLM采用基于深度优先搜索的决策树进行逐步推理，这可以实现捕捉API序列中的规律，但往往会导致用户无法接受的查询时间。
- **我们的方法：**  
  1. 我们的方法名为**SOAY**，它是一种基于解决方案的API使用方法论，旨在将LLM良好应用于学术信息检索/挖掘：
     - **解决方案生成：** SOAY首先让LLM根据用户输入生成一个可行的API调用计划，即解决方案，然后LLM会基于生成的解决方案生成可执行的API调用代码。
     - **避免重复推理：** 预生成的解决方案可以帮助LLM在生成后续代码时澄清学术API之间的复杂耦合关系，避免了重复推理，实现更接近传统学术搜索系统的效率水平。
     - **评估方法：** 为评估SOAY，我们引入了**SOAYEval**，一种同时考虑解决方案正确性和代码执行准确性的评估方法。
     - **有效性与效率：** 在人工评估和SOAYEval自动评估的共同评估体系下，我们验证了SOAY在使用AMiner API方面的有效性和效率以及在其它学术检索系统中应用的通用性。
- **项目成果：**  
  * 相关论文已完成，并已<u>录用于<u> **KDD 2025**（本科生作者之一）

---

## **💡💡💡 A Survey on Prompt Engineering: Taxonomy and Applications** <sub> &nbsp;&nbsp;[[Survey Paper]](https://baiyingzhuying.github.io/docs/LUNWENpromptengineering.pdf)</sub>

- **时间：** 2024.5 - 2024.12  
- **领域：** **LLM、Prompt Engineering**  
- **角色：** 本科生作者之一  
- **研究背景：**  
  1. 随着大语言模型（LLM）在各种下游任务中展现出卓越的性能，Prompt Engineering逐渐成为一个重要的研究领域，旨在优化用户与LLM之间的交互，以提高其整体性能。
  2. Prompt作为LLM的输入指令，与模型的响应密切相关，Prompt Engineering通过改进Prompt的内容和结构，增强了LLM的性能，而不需要修改模型本身的参数。
  3. 然而，目前关于Prompt Engineering的综述多集中于固定情景下的应用，如提升推理性能的Prompt Engineering，缺乏对Prompt Engineering技术和设计的全面总结。
- **我们的论文：**  
  1. 本文构建了一个全面的Prompt Engineering技术目录，并总结了这些技术在不同应用中的实际效果。
  2. 重点研究了离散前缀提示（discrete prefix prompts）而非填空提示（cloze prompts），因为利用前缀提示的现代LLM架构（尤其是decoder-only模型）在多个任务中表现出色。
  3. 主要关注硬性（离散）提示而非软性（连续）提示，并对Prompt Engineering的范围进行了细化，着重研究如何通过改变Prompt内容来提升模型性能。
- **项目成果：**  
  * 相关论文已完成，并已投递于 **TKDE 2025**（本科生作者之一）。

---

## **💡💡💡 Kaggle: LMSYS-Chatbot Arena Human Preference Predictions** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/lmsys-chatbot-arena) [[我们的方案]](https://github.com/baiyingzhuying/LMSYS_scheme_fyy)</sub>

- **时间：** 2024.5 - 2024.8  
- **领域：** **LLM微调、对话系统偏好预测**  
- **角色：** 团队(队长)  
- **研究背景：**  
  1. 本次比赛旨在通过预测用户在两个人工智能对话系统（LLM）之间的偏好，改进聊天机器人与人类的互动方式，使其更好地符合人类的偏好。
  2. 参赛者将获得来自Chatbot Arena的对话数据，这些数据由不同的LLM生成回答，挑战是开发一个能够准确预测用户偏好的机器学习模型。
- **我们的方案：**  
  1. 开发并优化了一种基于Gemma-2-9b-it模型的对话系统偏好预测模型，提升了用户偏好回复的预测精度：
     - **模型选择与尝试：** 选择Gemma-2-9b-it作为起始模型，测试过Llama3 8b、Llama3.1 8b等模型，效果不如Gemma-2，猜测原因是Gemma-2在ChatBot-1M数据集的后训练阶段已适应了该领域。
     - **合理的Prompt截断设计：** 设计了特殊的Prompt截断机制，在对话长度超过最大限制时，保证Prompt、Response A、Response B的比例合理，避免截断导致的信息丢失。
     - **LoRA微调与优化：** 使用LoRA对Gemma2ForSequenceClassification模型进行微调，将输出从传统的token预测改为分类任务。
     - **Test Time Augmentation策略：** 通过交换Response A和Response B的顺序，在推理阶段进行两轮预测并取平均，减少偏好带来的不平衡问题。
     - **特殊情况的后处理：** 针对log loss对极端值的敏感性，特别处理了Response为空或两者相同的特殊情况，优化了模型的表现。
- **项目成果：**  
  * 在1849支参赛队伍中位列第27名，摘得银牌&nbsp;|&nbsp;[证明](https://baiyingzhuying.github.io/docs/AWARDkaggleLMSYSSliver.png)

---

## **💡💡💡 Kaggle: LLM-Detect AI Generated Text** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/llm-detect-ai-generated-text)</sub>

- **时间：** 2023.11 - 2024.1  
- **领域：** **机器学习、LLM生成内容检测**  
- **角色：** 个人(Solo)  
- **研究背景：**  
  1. 随着大语言模型（LLM）的发展，它们生成的文本越来越难以与人类写作区分。本次竞赛旨在推动AI检测技术在实际应用中的研究与透明度。
  2. 参赛者需开发一个模型，准确判断文章是否由LLM生成。
- **我们的方案：**  
  1. 通过拼写错误修正来减少数据噪声。
  2. 使用KNN聚类筛选与测试数据集相似的训练数据集。
  3. 特征构建：训练Tokenizer+TF-IDF，构建稀疏矩阵embedding特征。
  4. 主体采用贝叶斯分类器、随机梯度下降分类器，并结合LGBM和CatBoost模型，提升整体Ensemble效果。
  5. 微调Deberta-v3-base模型，并在隐藏层后添加mean pooling层和线性分类层优化二分类任务。
  6. 最终方案为机器学习模型与Deberta模型的融合。
- **项目成果：**  
  * 在4358支参赛队伍中位列第222名，摘得银牌 (222 / 4358)&nbsp;|&nbsp;[证明](https://baiyingzhuying.github.io/docs/AWARDkaggleAIGenerateBronze.png)

---

## **💡💡💡 Kaggle: Optiver - Trading at the Close** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/optiver-trading-at-the-close)</sub>

- **时间：** 2024.1 - 2024.3  
- **领域：** **金融科技、AI for Trading**  
- **角色：** 团队(主力队员)  
- **研究背景：**  
  1. 股票收盘价对于全球经济至关重要。本次比赛挑战是开发一个模型，使用订单簿和股票收盘拍卖数据预测纳斯达克上市股票的收盘价走势。
- **我们的方案：**  
  1. 进行“特征工程”，包括特征转换、时序数据处理和特征选择。
  2. 尝试多种回归算法，如CatBoost、XGB、LGBM，最终选择LGBM。
  3. 使用Grid Search和Randomized Search方法优化超参数。
- **项目成果：**  
  * 在4436支参赛队伍中位列第223名，摘得银牌 (223 / 4436)&nbsp;|&nbsp;[证明](https://baiyingzhuying.github.io/docs/AWARDkaggleOptiverBronze.png)

---

## **💡💡💡 Reshaping Insurance&Preservation Model amidst Extreme Weather** <sub> &nbsp;&nbsp;[[比赛论文]](https://baiyingzhuying.github.io/docs/LUNWENmeisai.pdf)</sub>

- **时间：** 2024.2  
- **领域：** **数学建模**  
- **角色：** 团队(主力成员)  
- **研究背景：**  
  1. 极端天气事件给保险业带来了挑战和机遇，保险业需要改变经营模式以应对气候风险。
  2. 开发一个模型评估在极端天气地区承保的可行性，并为社区领导开发一个保护模型，以评估当地历史建筑的保护需求。
- **我们的论文：**  
  1. 提出以保险收益率为标准的决策模型。
  2. 使用层次分析法计算预期损失值(ELV)，并形成风险评估模型与损失评估模型。
  3. 根据预期收益率给出加州和甘肃的保险可行性建议。
  4. 综合分析并使用TOPSIS方法进行区域评分，最终得出“应增加对提高抗灾能力的投资”的结论。
- **项目成果：**  
  * 在2024年美国大学生数学建模竞赛(MCM/ICM)中获Meritorious Winner (国际一等奖，获奖率7.09%)

---

## **💡💡💡 基于贪心算法的多波束测量测线布设优化** <sub> &nbsp;&nbsp;[[比赛论文]](https://baiyingzhuying.github.io/docs/LUWENguosai.pdf)</sub>

- **时间：** 2023.9  
- **领域：** **数学建模**  
- **角色：** 团队(主力成员)  
- **研究背景：**  
  1. 海底探测中的多波束测深技术面临测线布设优化问题。测线间距过小会增加冗余数据，过大则降低地形分辨率，因此需要优化测线布设。
- **我们的论文：**  
  1. 建立了多波束测深覆盖宽度及相邻条带重叠率的数学模型。
  2. 提出最优测线布设方案，结合圆锥曲线模型优化测量效率。
  3. 通过MATLAB可视化数据并简化模型，利用贪心算法和深度优先搜索探索局部最优解，最终给出优良的测线设计方案。
- **项目成果：**  
  * 在2023年全国大学生数学建模竞赛中获北京赛区一等奖

# 🏆 Competition Achievements

- **Kaggle: Chatbot Arena Human Preference Predictions：银牌** *国家级* 2024 &nbsp;&nbsp;[[证明]]([https://btlazzq.github.io/docs/AWARDLMSYS.png](https://baiyingzhuying.github.io/docs/AWARDkaggleLMSYSSliver.png))  
- **Kaggle: LLM-Detect AI Generated Text：铜牌** *国家级* 2024 &nbsp;&nbsp;[[证明]]([https://btlazzq.github.io/docs/AWARDLLMDetect.png](https://baiyingzhuying.github.io/docs/AWARDkaggleAIGenerateBronze.png))  
- **Kaggle: Optiver - Trading at the Close：铜牌** *国家级* 2024 &nbsp;&nbsp;[[证明]]([https://btlazzq.github.io/docs/AWARDOptiver.png](https://baiyingzhuying.github.io/docs/AWARDkaggleOptiverBronze.png))  
- **美国大学生数学建模竞赛（MCM/ICM）：M奖** *国家级* 2024 &nbsp;&nbsp; [[证明]](https://example-link.com)
- **全国大学生数学建模竞赛（北京赛区）：一等奖** *省部级* 2023 &nbsp;&nbsp;[[证明]](https://example-link.com)
 
# 🥇 Scholarships and Honors

- **国家奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **学习优秀奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **优秀学生骨干奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **三好学生** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **优秀学生干部** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
