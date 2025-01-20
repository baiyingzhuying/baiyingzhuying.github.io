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

大家好！我是**付弋洋**，目前是本科三年级学生，就读于[中国人民大学](https://www.ruc.edu.cn)计算机科学与技术（图灵实验班）和金融科技实验班（高礼研究院）。

我对人工智能和金融科技充满热情，自入学以来，积极参与各类科研项目和学术竞赛，曾获得**国家奖学金**（2021-2022年）、**中国人民大学学习优秀奖学金**、**三好学生**、**优秀学生骨干奖学金**等荣誉。我的科研方向涵盖了**大语言模型与学术信息检索**、**深度学习应用**等领域。

# 🎓 Education Background

- **排名：** GPA 排名：**1/30**  
- **成绩均分：** GPA：3.84/4.0  
- **语言能力：** 英语能力优异，托福成绩为109/120（其中：阅读29/30，听力30/30），GRE成绩为321分。曾在加州大学戴维斯分校进行交换学习，且交换期间所有课程成绩均为满绩(A+/A)  
- **核心课程：** 高等数学 (91, 90)、高等代数 (93, 93)、数据结构与算法 (95, 93)、机器学习 (95)、数字信号处理 (95)、计算机系统基础 (90, 90)、编译原理 (92)、运筹学建模与算法 (94)  
- **编程能力：** 熟练掌握 C++、Python，熟悉算法与数据结构，抽象能力强，代码风格良好；熟练掌握 PyTorch、Numpy、Pandas，熟悉各类深度学习模型及其编程实现；具备优秀的编程/建模能力，多次获数学建模/数据挖掘比赛奖项（美赛M奖、Kaggle铜牌）  
- **开发工具：** VS Code，PyCharm，Jupyter Notebook，LaTeX (Overleaf)，Git  
- **在校荣誉：** 曾获 **国家奖学金**、中国人民大学学习优秀奖学金、中国人民大学优秀学生骨干奖学金、中国人民大学三好学生、中国人民大学优秀学生干部，在校累计获奖逾￥30000

# 🔍 Research Experience

## **💡💡💡 SOAY: A Solution-based LLM API-using Methodology for Academic Information Seeking** <sub> &nbsp;&nbsp;[[arXiv]](https://arxiv.org/abs/2405.15165) | [[Code]](https://github.com/RUCKBReasoning/SoAy) | [[Demo]](https://soay.aminer.cn/) </sub>

- **时间：** 2024.1 - 2024.8  
- **领域：** **LLM、AI4EDU**  
- **角色：** 合著者  
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
  * 相关论文已完成，并已录用于 **KDD 2025**（本科生作者之一）

---



# 🏆 **荣誉奖项**

- **Kaggle: Chatbot Arena Human Preference Predictions：银牌** *国家级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDLMSYS.png)  
- **Kaggle: LLM-Detect AI Generated Text：铜牌** *国家级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDLLMDetect.png)  
- **Kaggle: Optiver - Trading at the Close：铜牌** *国家级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDOptiver.png)  
- **美国大学生数学建模竞赛（MCM/ICM）：M奖** *国家级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDhulianwang+guo.pdf)  
- **全国大学生数学建模竞赛（北京赛区）：一等奖** *省部级* 2023 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDruanchuang_guo.pdf)
 
# 🥇 Scholarships and Honors

- **国家奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **学习优秀奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **优秀学生骨干奖学金** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **三好学生** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)
- **优秀学生干部** *中国人民大学* &nbsp;&nbsp;[[证明]](https://example-link.com)

# 📖 Educations
- **2022.09 - now**, 中国人民大学，北京，计算机科学与技术（图灵实验班），本科。
- **2023.02 - now**, 中国人民大学，北京，金融科技实验班（高礼研究院），本科（辅修）。
- **2023.09 - 2023.12**, 美国加利福尼亚州，UC Davis，计算机科学，交换生。
