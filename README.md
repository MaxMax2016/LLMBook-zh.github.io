# 大语言模型
作者：[赵鑫](<http://aibox.ruc.edu.cn/>)，[李军毅](<https://lijunyi.tech/>)，[周昆](<https://lancelot39.github.io/>)，[唐天一](<https://steventang1998.github.io/>)，[文继荣](<https://gsai.ruc.edu.cn/jrwen>)  

## 关于本书

2022年底，ChatGPT 震撼上线，大语言模型技术迅速“席卷”了整个社会，人工智能技术因此迎来了一次重要进展。面对大语言模型的强大性能，我们不禁要问：支撑这些模型的背后技术究竟是什么？这一问题无疑成为了众多科研人员的思考焦点。
必须指出的是，大模型技术并不是一蹴而就，其发展历程中先后经历了统计语言模型、神经网络语言模型、预训练语言模型等多个发展阶段，每一步的发展都凝结了众多科研工作者的心血与成果。作为大语言模型技术的重要推动者，OpenAI公司在过去深入探索了与其相关的大量技术细节，并最终推出了GPT系列模型，引领了本次技术变革。

然而，OpenAI 团队自GPT-3开始，就很少在公开的材料中提及相关技术细节，很多技术报告主要是介绍评测相关的内容。到目前为止，关于GPT系列模型的核心技术仍然难以完全解密。
目前，学术界面临的重大挑战是真正有充足资源去充分探索大语言模型训练的团队少之又少，因此导致了第一手经验匮乏，难以直接开展相关研究。
大模型训练涉及众多训练的细节，这些细节很多时候无法从已有科研论文中直接获取。由于其参数众多、组件复杂、训练过程也比较复杂，早期的实验探索如果不引入任何先验知识，可能会导致指数级增长的实验数量。这使得掌握大模型技术的经验变得尤为困难，更不用说从零开始探索相关科研问题，极大限制了学术界在此次人工浪潮中所起到的作用。
目前，能力较强的大语言模型基本都源自工业界，这一趋势随着时间的推移可能会变得更加明显。从第一手经验中“Know-How”，对于科研人员来说非常重要，只有接触到技术核心，才能真正理解哪些问题是有意义的，并找到解决方案。

令人欣喜的是，无论是在学术界还是工业界，人们都逐渐认识到了“开放”的重要性，能够看到越来越多的公开的基础模型、技术代码以及学术论文，有力地推动了大模型技术的“透明化”。只有通过开放和共享，才能汇聚全人类的智慧，共同推进人工智能技术的发展。实际上，根据现有公开的资料，大模型技术也是“有章可循”的，如整体训练流程、数据清洗方法、指令微调技术、人类偏好对齐算法等。根据这些技术，在算力资源支持下，研发人员已经能够较为顺利地完成大模型的整体训练流程，并取得不错的模型效果。随着更多核心技术的揭示和开放，大模型技术的“透明化”将进一步提高。

总之，大模型技术正处于快速发展阶段，基础原理亟待探索、关键技术亟待改善。对于科研人员而言，大模型研究工作充满了想象空间，令人为之神往。随着技术的不断进步与共享开放，我们有理由相信，未来人工智能技术将取得更大的进展，将在更多领域带来更为深远的影响。
本书旨在为读者提供关于大模型技术的全面了解，包括其基础原理、关键技术和应用前景。通过深入研究和实践，我们可以不断探索和改进大模型技术，为人工智能领域的发展做出贡献。
我们希望读者通过阅读本书，能够深入了解大模型技术的现状和未来趋势，为自己的研究和实践提供指导和启发。让我们携手努力，共同推动人工智能技术的发展，为建立更智能、更可持续的未来做出贡献。  

<br>
<div align="center">
  <img src="LLMbook-re.png" width="430" height="600">
</div>
<br>
  
## 本书内容

### 下载地址
**全书内容**： **《大语言模型》** (updated 2024-04-15)  
- 在2023年12月底，为了更好地提供大模型技术的中文参考资料，我们启动了中文书的编写工作，并且于近日完成初稿。中文版书籍注重为大模型技术的入门读者提供讲解，力图展现一个整体的大模型技术框架和路线图。本书适用于具有深度学习基础的高年级本科生以及低年级研究生使用，可以作为一本入门级的技术书籍。  
- [下载链接1](https://github.com/LLMBook-zh/LLMBook-zh.github.io/blob/main/LLMBook.pdf)，[下载链接2](http://aibox.ruc.edu.cn/zlwz/index.htm)

**英文综述论文**：[LLMSurvey](https://arxiv.org/abs/2303.18223)
- 为了更好地整理和传播大模型技术的最新进展与技术体系，我们在2023年3月发表了大语言模型英文综述文章《A Survey of Large Language Models》，并不断进行更新完善。这篇综述文章已经更新到第13个版本，包含了83页的正文内容，并收录了900余篇参考文献。
- 自英文综述文章上线后，陆续有读者询问是否有对应的中文版本。为此，我们于2023年8月发布了该综述（v10）的中文翻译版。  

### 配套资源
**LLMBox**： [代码库](https://github.com/RUCAIBox/LLMBox)  
- LLMBox是一个全面的代码工具库，专门用于开发和实现大语言模型，其基于统一化的训练流程和全面的模型评估框架。LLMBox旨在成为训练和利用大语言模型的一站式解决方案，其内部集成了大量实用的功能，实现了训练和利用阶段高度的灵活性和效率。

**YuLan大模型**： [代码库](https://github.com/RUC-GSAI/YuLan-Chat)  
- YuLan系列模型是中国人民大学高瓴人工智能学院师生共同开发的支持聊天的大语言模型（名字"玉兰"取自中国人民大学校花）。最新版本从头完成了整个预训练过程，并采用课程学习技术基于中英文双语数据进行有监督微调，包括高质量指令和人类偏好数据。

### 章节组织  
<div align="center">
  <img src="List.png" width="800" height="350">
</div>
<br>

## 引用信息  

```
赵鑫,李军毅,周昆,唐天一,文继荣，大语言模型，https://llmbook-zh.github.io/，2024.
```



```
@book{LLMBook,
  title = {大语言模型},
  year = {2024},
  author = {赵鑫, 李军毅, 周昆, 唐天一, 文继荣},
  address = {北京},
  url = {https://llmbook-zh.github.io/},
}
```

## 内容贡献表

本书各章节的主要负责人和参与人名单如下：

- 第三章的负责人是闵映乾和杨晨，参与人有李军毅、周昆； 
- 第四章的负责人是张君杰、侯宇蓬和周昆； 
- 第五章的负责人是董梓灿，参与人有田震和唐天一；
- 第六章的负责人是唐天一和陈昱硕；
- 第七章的负责人是唐天一，参与人有成晓雪；
- 第八章的负责人是李军毅和陈志朋；
- 第九章的负责人是陈昱硕、刘沛羽和唐天一，参与人有周昆；
- 第十章的负责人是李军毅、汤昕宇和都一凡，参与人有王晓磊；
- 第十一章的负责人是任瑞阳和蒋锦昊，参与人有李军毅；
- 第十二章的负责人是张北辰和周昆，参与人有张高玮；
- 第十三章的负责人是周昆，参与人（按拼音字母排序）有蒋锦昊、李依凡、刘子康、孙文奇、王禹淏、徐澜玲、杨锦霞和郑博文。

同时感谢其他参与本书编写、校对的同学，他们（按拼音字母排序）是曹乾、曹展硕、陈杰、程伽雅琪、戴孙浩、邓欣、丁毅杰、冯雪扬、高泽峰、苟志斌、辜子惠、郭歌扬、何东楠、侯新铭、胡译文、李炳黔、李成远、李欣潼、刘恩泽、刘炯楠、刘子涵、罗文扬、梅朗、欧柯杉、彭涵、阮恺、苏炜航、孙一丁、汤奕如、王家鹏、王磊、王淑婷、姚峰、尹彦彬、詹玉梁、张景森、张良、朱天宇和朱余韬。

本书在编写过程得到了中国人民大学大型科学仪器共享平台的算力资源支持，在此对于陈跃国、鲁蔚征、石源三位老师表示衷心的感谢。


## 反馈意见
在准备中文书的过程中，我们广泛阅读了现有的经典论文、相关代码和教材，从中提炼出核心概念、主流算法与模型，并进行了系统性的组织与介绍。
我们对于每个章节的内容初稿都进行了多次修正，力求表达的清晰性与准确性。
然而，在书写过程中，我们深感自身能力与知识的局限性，尽管已经付出了极大的努力，但难免会有遗漏或不当之处。本书的初版仅是一个起点，我们计划在网上持续进行内容的更新和完善，并特别欢迎读者提出宝贵的批评与建议，也会同步在网站上对于提出宝贵建议的读者进行致谢。我们将编写此书的过程当做一个自身的学习过程，也希望能够通过本书与读者进行深入交流，向更多的行业同行学习。

如果您有任何意见、评论以及建议（先确认最新版本中是否已经修正），请通过GitHub的[Issues](https://github.com/LLMBook-zh/LLMBook-zh.github.io/issues)页面进行反馈，或通过邮件发送至作者邮箱[rucaibox@163.com](rucaibox@163.com)。如果错误比较重要，我们会在本书中进行致谢。
