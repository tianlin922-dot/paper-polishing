# paper-polishing
## contents
- [一、总控 Prompt：整篇论文深度润色](#一总控-prompt整篇论文深度润色)
- [二、段落逻辑重构 Prompt](#二段落逻辑重构-prompt)
- [三、去中式英语 Prompt](#三去中式英语-prompt)
- [四、降低 AI 润色痕迹 Prompt](#四降低-ai-润色痕迹-prompt)
- [五、压缩啰嗦内容 Prompt](#五压缩啰嗦内容-prompt)
- [六、文献综述专用 Prompt](#六文献综述专用-prompt)
- [七、文献综述结构重组 Prompt](#七文献综述结构重组-prompt)
- [八、Introduction 专用 Prompt](#八Introduction-专用-prompt)









## 一、总控 Prompt：整篇论文深度润色
### 适合一开始把全文或整章交给模型时使用。
你是一名交通运输领域英文论文润色专家，熟悉 <你想投的期刊> 的写作风格。请对下面的论文内容进行深度润色。

总体目标：
1. 减少中式英语表达，使语言更接近英语母语学术写作；
2. 提高逻辑清晰度，使每段都有明确功能和自然衔接；
3. 减少口语化表达，但不要改成复杂长难句；
4. 降低 AI 润色痕迹，避免模板化表达，如 “This suggests that...”“Taken together...”“This is important because...” 的频繁重复；
5. 删除重复、啰嗦和泛化表达，使语言更凝练；
6. 保持 <你想投的期刊> 的政策导向，强调行为证据、政策含义、可实施性和适用边界；
7. 不改变原文事实、数据、变量名、方法和引用含义；
8. 如发现逻辑顺序不清，可以适当调整句子或段落结构。

请输出：
A. 润色后的英文版本；
B. 简要说明你主要修改了哪些方面；
C. 如果有明显逻辑问题或表达风险，请单独指出。
## 二、段落逻辑重构 Prompt
### 适合一段话读起来散、像堆句子时使用。
请不要只做逐句润色，而是先重构这段的逻辑。请按照“核心判断 → 证据或方法 → 解释机制 → 政策或研究含义” <按领域改> 的顺序重新组织下面这段内容。

要求：
1. 保留原有事实、数据和引用；
2. 删除重复解释和泛泛总结；
3. 让段落读起来像论文作者主动讨论结果，而不是机械复述模型输出；
4. 避免频繁使用 “This suggests that...”“This indicates that...”“This result shows...”；
5. 语言正式、清晰、自然，不要口语化，也不要写成长难句。
## 三、去中式英语 Prompt
### 适合任何读起来像中文直译的段落。
请重点检查下面文本中的中式英语表达，并将其改成自然、正式、地道的英文学术表达。

重点处理：
1. 中文式逻辑连接过多，如 “therefore / in this way / at the same time” 的机械使用；
2. 直译式表达，如 “the construction of...”“the promotion of...”“the development of...”；
3. 过度抽象或政策文件式表达；
4. 不自然的搭配和重复词；
5. 过长、过密、难读的句子。

请保持原意不变，使表达更适合交通运输领域英文期刊论文。
## 四、降低 AI 润色痕迹 Prompt
### 适合文本逻辑没问题，但读起来像 AI 改过。
这段文字逻辑基本正确，但读起来有明显 AI 润色痕迹。请重新润色，使其更像论文作者自然写出的英文。

请重点减少：
1. 模板化句式，如 “This suggests that...”“This finding highlights...”“Taken together...”；
2. 过度整齐的句子结构；
3. 泛化表达，如 “provides a structured pathway”“has important implications”“plays a crucial role”；
4. 机械的“结果—意义—政策建议” <按领域改> 句式；
5. 不必要的抽象名词堆叠。

要求：
语言正式但自然，句式有变化，逻辑清楚，避免口语化，不要牺牲学术性。
## 五、压缩啰嗦内容 Prompt
### 适合 introduction、literature review、methodology 或 discussion 太长时使用。
请在不丢失核心信息的前提下压缩下面内容。

压缩原则：
1. 删除重复解释、泛泛铺垫和可以留到其他章节的细节；
2. 合并功能相近的句子；
3. 保留核心研究问题、方法、关键发现和政策含义；
4. 保持英文自然流畅；
5. 不要压缩成过于抽象的概念句；
6. 避免长难句。

请输出一个更凝练、更适合期刊正文的版本。
## 六、文献综述专用 Prompt
### 适合 literature review 的整体润色。
请将下面的文献综述改写得更像成熟的英文期刊 literature review，而不是文献罗列。

要求：
1. 每段围绕一个清晰的中心判断展开；
2. 减少“某某研究发现...”的流水账式写法；
3. 用综合性语言概括一类研究解决了什么问题、仍缺什么；
4. 保留原有引用，不新增虚构文献；
5. 减少重复词，如 adoption, factors, attributes, evidence, policy design <按领域改> ；
6. 用 drivers, constraints, mechanisms, conditions, barriers, public response, uptake <按领域改> 等词适当替换；
7. 最后一节要明确本文定位：已有研究能解释什么，但尚未解决什么；本文如何补充。
8. 保持语言正式、凝练、易读，减少中式表达和 AI 模板句。
## 七、文献综述结构重组 Prompt
### 适合文献综述结构混乱时使用。
请根据下面内容重新组织 literature review 的结构。
<以下内容建议自我总结梳理后改>
建议结构：
2.1 Evidence on eVTOL adoption and public acceptance
重点综述 eVTOL 接受度、服务表现、安全信任、价格、接驳、基础设施和用户异质性。

2.2 Methods for adoption analysis and policy-oriented reasoning
重点综述 SP surveys 的价值与局限、相似新兴交通方式的政策经验、LLM/KG 方法对政策推理的作用。

2.3 Study positioning
明确指出现有研究较强于解释 adoption/acceptance，但较弱于将行为证据转化为 policy design。然后说明本文如何通过 survey evidence, KG, and LLM 连接 public concerns 和 policy recommendations。

要求：
1. 不要混淆 eVTOL 和 UAM，eVTOL 是本文核心对象，UAM 只作为更宽背景；
2. 不要写成文献清单；
3. 保留原引用；
4. 语言更 native、更凝练。
## 八、Introduction 专用 Prompt
### 适合引言整体润色。
请将下面的 introduction 改写成更适合 <你想投的期刊> 的版本。
<以下内容建议自我总结梳理后改>
逻辑要求：
1. 第一段说明 eVTOL 的交通意义，但不要过度宣传；
2. 第二段说明公众接受、安全、信任、价格和监管问题；
3. 第三段说明 SP survey 的价值和局限，以及为什么需要结构化政策知识；
4. 第四段说明本文如何回应 gap：survey evidence → knowledge graph → LLM reasoning → policy recommendations；
5. 最后一段贡献点要清楚，避免抽象表达。

语言要求：
1. 减少中式英语；
2. 避免长难句；
3. 不要写得像 AI 润色；
4. 不要重复 eVTOL adoption / policy design / evidence 等词；
5. 保持正式、简洁、政策导向。
