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

<font face="Times New Roman">
<div style="text-align: center; margin-bottom: 30px;">
    <h1 style="font-family: Georgia, serif; font-size: 2.5em; color: #2a4d69;">刘一澎</h1>
    <p style="font-size: 1.25em; color: #4b86b4;">
        <a href="https://xxxy.lzu.edu.cn/" style="color: #4b86b4; text-decoration: none;">兰州大学信息科学与工程学院</a> · 计算机科学与技术专业 · 本科三年级
    </p>
    <hr style="width: 100%; border: 1px solid #4b86b4;">
</div>

<p style="text-align: justify; font-size: 1.15em; margin-bottom: 30px;">
    大家好！我是 <b>刘一澎</b>，目前是本科三年级学生，专注于人工智能和计算机科学的交叉研究领域。
    自入学以来，我积极参与各类科研项目和学术竞赛，并获得了多项荣誉与奖项。我特别关注
    <b>图神经网络</b>、<b>计算机视觉</b>、<b>大语言模型</b>、以及<b>人工智能安全</b>等领域的前沿研究。
</p>

<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">🎓 教育背景</h2>
<ul style="font-size: 1.15em; margin-bottom: 30px;">
    <li><b>排名：</b> GPA排名：<b>2/108 (1.8%)</b>、加权平均分排名：<b>2/108 (1.8%)</b></li>
    <li><b>成绩均分：</b> GPA：4.03/5.0、加权平均分：90.11/100</li>
    <li><b>语言能力：</b> 通过 CET4 和 CET6，独立撰写并发表两篇全英学术论文（均已被录用）</li>
    <li><b>核心课程：</b> 高等数学 (93)、线性代数 (97)、商务统计（即: 概率论与数理统计） (94)、数据结构 (97, 95)、计算机编程 (理论) (94, 100)、计算机编程 (实践) (97, 100)、数据管理 (99, 96)、信息可视化 (97)</li>
    <li><b>编程能力：</b> 精通 C/C++ 和 Python，熟悉算法与数据结构；精通深度学习模型的实现，长期担任数学建模编程手</li>
    <li><b>开发工具：</b> VS Code, PyCharm, Jupyter Notebook, LaTeX (Overleaf), Git</li>
    <li><b>在校荣誉：</b> 国家奖学金获得者 
        <a href="https://samer-hue.github.io/docs/guojiang.pdf" style="font-size: 0.8em; color: #4b86b4;">[国奖证书]</a>，
        兰州大学优秀学生一等奖学金，兰州大学学生标兵称号
    </li>
</ul>


<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">🧠 研究经历 (主要) (图学习)</h2>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">DicTED-预训练嵌入蒸馏增强字典图神经网络</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://samer-hue.github.io/DicTED/README.html" style="color: #4b86b4;">[项目主页]</a> | <a href="https://github.com/Samer-hue/DicTED" style="color: #4b86b4;">[项目代码]</a> | <a href="https://link.springer.com/chapter/10.1007/978-981-97-5678-0_29" style="color: #4b86b4;">[论文链接]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2023.03 - 2024.03</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 图学习</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 独立第一作者</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>时序图学习通过将时间维度纳入分析(引入了新的技术来建模和分析图的时间动态)扩展了传统图学习方法的能力。然而，数据结构的约束往往导致现有方法中获取多源信息的复杂性极高，频繁的更新和训练也常会致使记忆问题。</li>
        <li>为了解决上述挑战，出现了一类称为字典时序图网络的技术。这种方法聚集邻域信息并将其存储为字典，然后根据需要进行匹配和提取，与现有方法相比，字典网络在训练过程中可以更加灵活地存储、更新和计算，从而获得更好的性能。</li>
        <li>然而，字典时序图网络虽然可以方便地存储更新的嵌入信息，但在初始化阶段严重依赖于图数据的特征。如果没有可靠的特征集，模型往往会陷入冷启动问题，从而对后续的训练结果产生负面影响或大大延长训练时间。同时，字典中的嵌入信息是不断更新的，在训练过程中，由于新知识不断覆盖已有知识，模型会在训练后期逐渐失去对旧知识的掌握，并往往会致使灾难性遗忘问题，这对模型全面获取信息的能力产生了重大挑战。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的方法：</b></p>
    <ul style="font-size: 1.15em;">
        <li>构建基于预训练嵌入蒸馏的字典时序图网络(DicTED)，引入多个预训练的教师模型来生成嵌入，然后将其融合为DicTED的先验特征，在不过度增加模型复杂性的前提下，有效地解决了上述问题。</li>
        <li>输入端：将先验特征与原始特征相结合，增强模型初始化，使模型在训练中获得更可靠的信息,成功解决训练前期的冷启动问题。</li>
        <li>优化端：优化模型的嵌入损失和预测分数损失，促使训练节点嵌入与先验特征尽可能对齐，从而尽可能地保留原始信息，成功解决训练后期的灾难性遗忘问题。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 在多个真实数据集上的实验表明，DicTED优于现有的SOTA方法。</p>
</div>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">基于拓扑能量的联邦图后门攻击防御策略</h3>
    <p style="font-size: 1.15em;"><b>时间：</b> 2024.04 - 2024.08</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 联邦图学习</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 共同第一作者</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>联邦图学习(FGL)通过允许多个客户端在保护敏感数据隐私的同时协同训练共享的全局模型，为分布式图数据的建模和分析提供了新的范式。</li>
        <li>FGL的分布式特性也引入了新的漏洞，特别是来自恶意参与者的后门攻击，这些攻击会在训练过程中注入有害数据或模型，从而在特定条件下触发错误的模型输出。</li>
        <li>图数据通常表现出非IID特性和复杂的拓扑结构，致使联邦学习中针对后门攻击的防御方法在FGL环境下往往难以有效发挥作用。</li>
        <li>另外一些方法试图简单地计算客户端之间的距离或某些分布的相似性，而没有任何额外的处理来区分恶/良性客户端，使得其仍然是耦合的。同时，大多数方法没有充分考虑数据异质性给它们测量的指标带来的额外挑战。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的方法：</b></p>
    <ul style="font-size: 1.15em;">
        <li>引入了一种基于能量视角的创新框架，从微观和宏观两个层面来解决上述问题。</li>
        <li>在微观层面，引入拓扑能量客户端聚类TNC来解决复杂拓扑触发器问题：TNC量化了客户端数据分布的差异，将全面的分布感知注入到局部模型中，使其现有的预测能力与辨别数据能量分布的能力相结合。</li>
        <li>在宏观层面，提出了拓扑能量相似性TSP，进一步解耦恶意和良性客户端的能量分布：收集每个客户端的能量分布，并基于客户端上传的能量分布的相似性建立能量图。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究进度：</b></p>
    <ul style="font-size: 1.15em;">
        <li>在IID / 非IID场景下的五个主流数据集上进行了实验，结果表明我们的方法优于目前的SOTA。</li>
        <li>当前工作已进入实验收尾阶段，论文写作中，预计投稿至ICLR 2025。</li>
    </ul>
</div>


<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">🖥️ 研究经历 (其它) (计算机视觉、大语言模型、可视化)</h2>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">FreeMRISeg-磁共振图像分割</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://samer-hue.github.io/MRI-Segmentation/README.html" style="color: #4b86b4;">[Homepage]</a> | <a href="https://github.com/Samer-hue/MRI-Segmentation" style="color: #4b86b4;">[Code]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2022.9 - 2022.12</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 计算机视觉、医工交叉</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队负责人</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>深度学习技术近年来在医学图像处理方面展现出了优秀的能力，其在磁共振成像(MRI)扫描或计算机断层扫描(CT)上往往可以对患者的病变进行有效的定位和分割。</li>
        <li>然而，训练这些分割模型需要大量专业医生手动标注的像素级标签，这与更容易获得的图像级标签相比更加耗时且费力。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的方法：</b></p>
    <ul style="font-size: 1.15em;">
        <li>设计了一个使用图像级标签作为监督的弱监督语义分割模型解决了这一问题，其主要包含[分类]、[分割]两部分。</li>
        <li><b>分类任务部分：</b> 首先使用选定的卷积神经网络（在AlexNet、GoogLeNet、VGG、ResNet中测试效果，最终选择ResNet）对公开的已有图像级标签数据集（如：RSNA2019）进行分类训练，之后使用CAM推理判断分类网络关注点并从CAM图得到Mask，同时使用CRF优化mask，得到像素级标签并和专家标注的ground mask比较效果。</li>
        <li><b>分割任务部分：</b> 使用分类任务得到的像素级标签来训练分割网络（backbone选取Deeplabv3、Trans-Unet、Swin-Unet、MT-Unet），完成整个弱监督分割工作流。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 该科研课题成功申请为“中央高校基本科研业务专项资金”本科生项目。</p>
</div>


<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">面向高效多租户LoRA服务的动态算子优化</h3>
    <p style="font-size: 1.15em;"><b>时间：</b> 2024.7 - 2024.8</p>
    <p style="font-size: 1.15em;"><b>领域：</b> Efficient AI、高效微调</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 第三作者</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>低秩自适应(LoRA)已经成为在资源和数据受限的条件下，有效微调LLM的关键技术传统。</li>
        <li>传统上，我们需要独立处理每个LoRA模型，这会导致冗余的存储和计算，特别是当多个模型共享相同的预训练主干时，因为源自相同预训练模型的一些LoRA模型之间的存在潜在的权重相关性。</li>
        <li>当今的方法如vLLM和FastTransformer无法同时处理多个LoRA模型因为它们不能有效地批量处理不同模型的GPU操作。</li>
        <li>Punica通过引入了名为分段聚合矩阵向量乘法(SGMV)的新颖算子，做到了为不同的LoRA模型进行批量GPU操作，但其核心算子的实现不具备灵活性和多样性，往往使用通用方法实现，这可能不是特定任务和硬件架构的最佳选择。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的方法：</b></p>
    <ul style="font-size: 1.15em;">
        <li>引入动态算子优化来解决上述问题:其旨在基于特定场景动态优化SGMV算子。</li>
        <li>具体实现上，其利用搜索空间构造器创建分层搜索空间，将程序空间划分为高维的结构草图和低维的实现细节，确保了操作符实现的多样性和灵活性。</li>
        <li>优化引擎将在估算程序性能的成本模型指导下，使用进化搜索改进算子的实现，这种迭代优化过程确保SGMV的实现可以动态适应不同的场景，以保持高性能。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 目前实验效果较为良好: 将我们的方法应用于最先进的服务系统可以实现1.30-1.46倍的吞吐量提高。</p>
</div>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">Kaggle: LMSYS-Chatbot Arena Human Preference Predictions</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://www.kaggle.com/competitions/lmsys-chatbot-arena" style="color: #4b86b4;">[比赛介绍]</a> | <a href="https://www.kaggle.com/competitions/lmsys-chatbot-arena/leaderboard" style="color: #4b86b4;">[Leaderboard]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2024.5 - 2024.8</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 大语言模型、模型微调</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队主力成员</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>本次比赛中，参赛者将被挑战去预测用户在与两个由大语言模型(LLM)驱动的聊天机器人之间的交谈中更喜欢哪些回答。</li>
        <li>参赛者将获得一组来自Chatbot Arena的对话数据，这些对话由不同的LLM生成回答。通过开发一个满足任务要求机器学习模型，帮助改进聊天机器人与人类互动的方式，确保它们更好地符合人类的偏好。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的方法：</b></p>
    <ul style="font-size: 1.15em;">
        <li>先后测试了Deberta base、Deberta v2、Xlarge、Deberta v3 large等“小语言”模型，发现效果不尽如人意。</li>
        <li>查阅了一些公开方案和讨论区的观点，发现这场比赛使用“大语言”模型可能更合适。因此在而后又尝试了Gemma2 9b，Gemma2 27b，Llama3 8b模型。</li>
        <li>Gemma2 27b在本地进行测试时的表现最好，但是会超出比赛环境的GPU显存，所以最终选择了Gemma2 9b和Llama3 8b模型。</li>
        <li>在确定模型后，使用QLoRA对这两个模型进行微调，并尝试了两种方案: [对Gemma2 9b设置较高的Rank（32,64）进行微调，并作为单模型] / [对Gemma2 9b和Llama3 8b均设置较低的Rank（16）进行微调，最终进行Ensemble]，最终根据结果选取后一种方案。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 摘得本次竞赛的银牌（Top 5%）。</p>
</div>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">从“堆盒子”到动态规划</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://www.bilibili.com/video/BV1ojKvehEuq" style="color: #4b86b4;">[Bilibili页面]</a> | <a href="https://github.com/mumuyeye/From-Stacking-Boxes-to-Dynamic-Programming" style="color: #4b86b4;">[Code]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2023.9 - 2023.12</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 算法可视化、算法教学</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队主力成员</p>
    <p style="font-size: 1.15em;"><b>研究背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>算法学习一直是很多投身于算法竞赛的高中生和计算机相关专业大学生的一块“心病”。</li>
        <li>算法教学领域存在诸多通病——有些课程要么浅尝辄止，难以让同学们从本质上掌握并能熟练运用算法知识，要么过于专业和晦涩，让同学们听的一头雾水。</li>
        <li>“化抽象为具象”的最佳方法便是对算法进行“可视化”。</li>
        <li>Manim是一款基于python的数学动画制作引擎，由斯坦福大学的数学系学生Grant Sanderson创建，并用于YouTube频道3Blue1Brown，来解说高等数学。</li>
        <li>Manim可以快速构建非常精彩而又形象的动画，例如数学证明可视化、数学运算可视化、二/三维模型可视化、机械原理可视化，Manim都可以精彩完成。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的作品：</b></p>
    <ul style="font-size: 1.15em;">
        <li>采用了与著名博主3Blue1Brown所同源的基于Python的数学动画制作引擎Manim来制作，自主编写3000余行代码，配合后期大量的代码微调、剪辑、AI处理搭配工作，最终得以完成本次作品。</li>
        <li>其以更完整的教学结构、更通俗易懂的讲解、更专业的可视化（使用专业的Manim引擎而非传统的动画制作软件）、更友好的教学模式以及更具创新性的教学理念，在Coding for Education领域真正走到了前沿。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 将视频发布到了Manim爱好者的交流社群中，在本院同学之间进行测试反馈和迭代，再到各高中乃至高校进行应用推广，均收到了良好反馈。</p>
</div>



<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">📊 数学建模经历</h2>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">母亲身心健康对婴儿睡眠质量的影响分析</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://samer-hue.github.io/docs/huashubei23C.pdf" style="color: #4b86b4;">[项目报告]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2023.7 - 2023.8</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 数学建模、关联分析、多目标优化</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队队长</p>
    <p style="font-size: 1.15em;"><b>建模背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>母亲的不良心理健康状态往往会对婴儿的认知情感等方面产生负面影响，因此，围绕母亲的身体心理指标与婴儿的睡眠指标之间的关系进行建模十分重要，其有利于提高母亲的心理健康水平、促进婴儿的生理心理上的健康发展。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的论文：</b></p>
    <ul style="font-size: 1.15em;">
        <li>建立SEM模型，将母亲的身体和心理指标作为自变量，婴儿行为和睡眠质量作为因变量，分析路径系数，揭示母亲因素对婴儿的影响。</li>
        <li>使用基于熵权法的TOPSIS模型量化身体和心理指标，并结合Adaboost、GBDT和随机森林构建Soft Voting分类器，预测婴儿行为特征，模型准确率达95%以上。</li>
        <li>构建MIMO神经网络模型，输入母亲特征预测CBTS、EPDS和HADS得分，模型拟合优度达96.4%。</li>
        <li>将婴儿睡眠质量的四分类任务视为无监督学习问题，采用K-means算法聚类，并通过TOPSIS模型和Soft Voting模型验证分类结果的合理性，模型准确率达91.6%。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 作为队长组织团队参加2023年“华数杯”全国大学生数学建模竞赛，并获全国一等奖。</p>
</div>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">基于计算几何和遗传算法的多波束测深和测线布设模型</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://samer-hue.github.io/docs/shumoguosai23B.pdf" style="color: #4b86b4;">[项目报告]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2023.8 - 2023.9</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 数学建模、计算几何、多目标优化</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队队长</p>
    <p style="font-size: 1.15em;"><b>建模背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>传统海洋测绘常用单波束测深系统，但在地形复杂处需多次测量，且对测量人员要求较高; 在现代海洋测绘中，高效率、高精度、全覆盖的多波束测深系统被更加广泛地应用; 为了使得多波束测深系统能够更加准确地测出数据，设计合适的测线显得极其重要。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的论文：</b></p>
    <ul style="font-size: 1.15em;">
        <li>通过多波束测深模型测量海底深度，并运用遗传算法优化海测线布设。</li>
        <li>应用平面几何定理计算测深覆盖宽度和重叠率等公式，并依数据求出真实值。</li>
        <li>将测量船与海底坡面的位置关系抽象为三棱锥体，利用立体几何定理分析不同测线夹角下的测深覆盖宽度与船距中心点的关系。</li>
        <li>设计两种测线布设方案，通过几何公式和Bisinhopping算法求出最优解。</li>
        <li>根据数据生成海底地形仿真图。</li>
        <li>使用贪心算法将三个目标函数归一化，建立加权目标函数。</li>
        <li>通过遗传算法多次迭代，得到最终解。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 作为队长组织团队参加2023年“高教社杯”全国大学生数学建模竞赛，并获省级一等奖。</p>
</div>

<div style="margin-bottom: 30px;">
    <h3 style="font-family: Georgia, serif; font-size: 1.75em; color: #2a4d69;">基于仿真模拟的三角形纯方位无源定位模型</h3>
    <p style="font-size: 1.15em;"><sub><a href="https://samer-hue.github.io/docs/shumoguosai22B.pdf" style="color: #4b86b4;">[项目报告]</a></sub></p>
    <p style="font-size: 1.15em;"><b>时间：</b> 2022.8 - 2022.9</p>
    <p style="font-size: 1.15em;"><b>领域：</b> 数学建模、仿真模拟</p>
    <p style="font-size: 1.15em;"><b>角色：</b> 团队队长</p>
    <p style="font-size: 1.15em;"><b>建模背景：</b></p>
    <ul style="font-size: 1.15em;">
        <li>无人机在当今的民用和军用方面都有很大的作用。在军用中,无人机常以编队的形式执行任务，此时，为避免被外界干扰以及被雷达探测，应当减少电磁信号的传播。因此如何在不同编队队形中通过无源探测定位的方式来有效调整无人机的位置显得尤为重要。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>我们的论文：</b></p>
    <ul style="font-size: 1.15em;">
        <li>通过建立三角形纯方位无源定位模型确定圆形编队中无人机的位置，并通过仿真模拟验证模型的有效性，应用于不同编队。</li>
        <li>为确定接收信号无人机的位置，建立三角形定位模型，假设角度测量呈正态分布，测量点位于某定位三角形中，通过仿真生成10000个正态分布点，计算它们与重心和内心的平均距离，最终选用内心代表测量点位置。</li>
        <li>建立四点定位模型，四架无人机发射信号形成4个定位三角形，测量点处于4个三角形相交的公共区域内，面积小于任一三角形，从而减少误差，并通过计算4个三角形内心坐标的平均值有效定位无人机位置。</li>
    </ul>
    <p style="font-size: 1.15em;"><b>研究成果：</b> 作为队长组织团队参加2022年“高教社杯”全国大学生数学建模竞赛，并获省级一等奖。</p>
</div>


<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">🏆 竞赛奖项</h2>

<ul style="font-size: 1.15em;">
    <li>
        <b>Kaggle: Chatbot Arena Human Preference Predictions：银牌</b> 
        <a href="https://www.kaggle.com/competitions/lmsys-chatbot-arena/leaderboard" style="font-size: 0.8em; color: #4b86b4;">[Leaderboard]</a>
        <b>国家级</b> 2024
    </li>
    <li>
        <b>中国机器人及人工智能大赛(全国总决赛)：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDCRAICguo.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>国家级</b> 2024
    </li>
    <li>
        <b>“华数杯”全国大学生数学建模竞赛：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDhuashubei.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>国家级</b> 2023
    </li>
    <li>
        <b>全国大学生数据统计与分析竞赛：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDshujutongjifenxi.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>国家级</b> 2023
    </li>
    <li>
        <b>“英语世界”杯全国大学生英语语法大赛：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDenglishgrammar.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>国家级</b> 2023
    </li>
    <li>
        <b>“互联网＋”大学生创新创业大赛：金奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDhulianwang+.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>省部级</b> 2023
    </li>
    <li>
        <b>全国大学生数学建模竞赛：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDshumoguosai23.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>省部级</b> 2023
    </li>
    <li>
        <b>全国大学生数学建模竞赛：一等奖</b> 
        <a href="https://samer-hue.github.io/docs/AWARDshumoguosai22.pdf" style="font-size: 0.8em; color: #4b86b4;">[证明]</a>
        <b>省部级</b> 2022
    </li>
</ul>


<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">🥇 奖学金与荣誉</h2>

<ul style="font-size: 1.15em;">
    <li>
        <b>2021-2022</b> <b>国家奖学金</b> (该年度年级成绩排名：1/108) 
        <a href="https://samer-hue.github.io/docs/guojiang.pdf" style="font-size: 0.8em; color: #4b86b4;">[国奖证书]</a> 
        <b>兰州大学</b>
    </li>
    <li>
        <b>2021-2022</b> <b>兰州大学优秀学生一等奖学金</b> (获奖率：3%) 
        <b>兰州大学</b>
    </li>
    <li>
        <b>2021-2022</b> <b>兰州大学学生标兵</b> 
        <b>兰州大学</b>
    </li>
</ul>

<h2 style="font-family: Georgia, serif; color: #2a4d69; border-bottom: 2px solid #4b86b4; padding-bottom: 5px;">📖 教育经历</h2>

<ul style="font-size: 1.15em;">
    <li><b>2021.9 -</b>, 本科生, 兰州大学信息科学与工程学院 · 专业：计算机科学与技术</li>
</ul>
</font>
