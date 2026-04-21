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
- [九、贡献点润色 Prompt](#九贡献点润色-prompt)
- [十、Methodology 专用 Prompt](#十Methodology-专用-prompt)
- [十一、Results and Discussion 专用 Prompt](#十一results-and-discussion-专用-prompt)
- [十二、Policy Implications 专用 Prompt（仅适用于特定方向）](#十二policy-implications-专用-prompt仅适用于特定方向)
- [十三、Conclusion 专用 Prompt](#十三conclusion-专用-prompt)
- [十四、Abstract 专用 Prompt](#十四abstract-专用-prompt)
- [十五、题目生成 Prompt](#十五题目生成-prompt)
- [十六、表格标题和表头润色 Prompt](#十六表格标题和表头润色-prompt)
- [十七、References 标准化 Prompt](#十七references-标准化-prompt)
- [十八、自动迭代优化 Prompt 模板](#十八自动迭代优化-prompt-模板)
- [十九、最终通篇检查 Prompt](#十九最终通篇检查-prompt)
- [二十、带高亮修改 Prompt](#二十带高亮修改-prompt)







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
## 九、贡献点润色 Prompt
### 适合 contributions 写得抽象时使用。
请重新润色下面的 contribution paragraph，使每个贡献点更清楚、更具体。

<以下内容建议自我总结梳理后改>

要求：
1. 不要只写抽象判断，如 “treats eVTOL as both a behavioral and policy problem”；
2. 每个贡献点要说明本文具体做了什么；
3. 第一贡献点应强调：本文不是只测量接受度或预测需求，而是把 adoption barriers 连接到 policy design；
4. 第二贡献点应强调：KG 作为 SP evidence 和 LLM reasoning 之间的中间层，提高约束性和可解释性；
5. 第三贡献点应强调：借鉴相似新兴交通方式的政策经验，形成可扩展的早期政策设计框架；
6. 语言简洁，不要过度拔高。
## 十、Methodology 专用 Prompt
### 适合方法章节太流水账、口语化时使用。
请润色下面的 methodology，使其更像正式英文期刊的方法章节。

要求：
1. 先说明方法设计逻辑，再说明具体步骤；
2. 减少 “First, Second, Third” 的机械说明；
3. 将重复的小步骤适当合并；
4. 保留公式、变量定义、模型假设和关键流程；
5. 语言正式、清楚、可复现；
6. 避免口语化表达，如 “the next step”“this process has three stages”；
7. 不要写成 AI 工具说明书；
8. 对 <组合模块> 的描述要强调它们在本文方法中的功能，而不是泛泛介绍技术。
## 十一、Results and Discussion 专用 Prompt
### 适合结果和讨论部分整体润色。
请将下面的 Results and Discussion 改写得更适合 <你想投的期刊>。

<以下内容建议自我总结梳理后改>

要求：
1. 每段先给出核心发现，再解释机制，最后自然引出政策含义；
2. 不要机械罗列系数；
3. 减少 “A affects B, indicating...” 的重复句式；
4. 政策建议必须有结果依据，不要泛泛建议；
5. 增加适度的讨论深度，包括可信度、适用边界和政策依据；
6. 避免口语化表达；
7. 降低 AI 味道，不要频繁使用模板句；
8. 保留关键系数、显著性结论和图表引用。
## 十二、Policy Implications 专用 Prompt（仅适用于特定方向）
### 适合政策建议像清单时使用。
请重写下面的 policy implications，使其逻辑更集中，不像建议清单。

建议主线：
1. 对 policymakers：透明安全治理、差异化沟通、门到门可达性；
2. 对 operators：价格门槛、全链条服务体验、用户认知建立；
3. 每条建议都要对应前文结果，而不是泛泛提出；
4. 说明适用边界，避免过度泛化；
5. 语言正式、简洁，不要口语化；
6. 减少 “should therefore” 的重复使用。
## 十三、Conclusion 专用 Prompt
### 适合 conclusion 过散、过抽象时使用。
请将下面的 conclusion 重新组织为四个部分：

1. 本文做了什么；
2. 模型或方法表现如何；
3. 得到哪些关键结论；
4. 未来研究方向。

要求：
1. 不要把背景、方法、贡献、政策建议、局限全部散开堆放；
2. 减少抽象表达，如 “systematic framework”“broader relevance”“structured pathway”；
3. 用更具体的语言说明研究发现和意义；
4. 未来研究要具体，如扩展知识图谱、更多城市验证、从首次使用到持续使用<建议总结后更换>；
5. 语言凝练、正式、自然。
## 十四、Abstract 专用 Prompt
### 适合摘要润色和拔高。
请根据论文内容撰写或润色 abstract，使其适合 <你想投的期刊>。

<以下内容建议自我总结梳理后改>

结构要求：
1. 研究背景：eVTOL 的交通意义和部署挑战；
2. 研究缺口：已有研究关注接受度和需求，但 behavioral evidence 与 policy design 的连接不足；
3. 方法：SP survey, causal network, knowledge graph, and KG-enhanced LLM；
4. 数据：说明样本来源和核心规模；
5. 结果：概括主要影响因素和模型比较结果；
6. 政策意义：安全治理、价格可达性、门到门整合、差异化沟通；
7. 贡献：连接 public acceptance analysis 与 policy design。

语言要求：
1. 不要太简单；
2. 不要过度抽象；
3. 不要重复 large language model；
4. 避免中式英语；
5. 控制在 180–250 词左右。
## 十五、题目生成 Prompt
### 适合生成投稿标题。
请基于下面论文内容生成 8–10 个英文标题，适合 <你想投的期刊>。

要求：
1. 标题要突出交通政策问题，而不只是 AI 技术 <跟据你的主题更改> ；
2. 体现 public acceptance / behavioral evidence / policy design / eVTOL deployment <跟据你的主题更改> ；
3. 可以提供陈述式和疑问句两类；
4. 不要过度夸张；
5. 不要显得像新闻标题；
6. 避免直接照搬特刊标题或关键词；
7. 给出你最推荐的 2 个标题，并说明理由。
## 十六、表格标题和表头润色 Prompt
### 适合表格表达不地道时使用。
请润色下面表格的标题、列名和表述，使其更符合英文期刊写法。

要求：
1. 表题简洁、准确；
2. 列名使用自然学术表达；
3. 删除中式或直译表达，如 “Information on...”；
4. 统一大小写和术语；
5. 不改变表格含义；
6. 如有更地道的替代表达，请给出。
## 十七、References 标准化 Prompt
### 适合参考文献格式统一。
请按照以下格式统一整理参考文献：

Author A, Author B, Author C, et al. Title[J]. Journal Name, Year, Volume(Issue): Page range / Article number.

要求：
1. 保留原文献顺序，除非我要求按字母排序；
2. 补充缺失的期刊全名、卷号、期号、页码或文章编号；
3. 统一作者格式，去掉不一致的括号格式；
4. 统一 [J] 格式；
5. 题名大小写保持 sentence case；
6. 如果某条信息无法确认，请标注“需要核对”，不要编造；
7. 如果发现明显与论文主题不相关的参考文献，请单独提醒。
## 十八、自动迭代优化 Prompt 模板
### 这个适合你把一整节反复丢给模型自动优化。
请对下面文本进行三轮自动迭代润色。

第一轮：诊断
请指出文本中的主要问题，包括逻辑松散、中式英语、重复词、口语化表达、AI 模板句、过度抽象、段落功能不清等。

第二轮：结构优化
请在不改变原意、数据、引用和方法的前提下，重新组织段落逻辑，使其更符合英文交通运输期刊论文的写法。

第三轮：语言精修
请进一步提升语言质量，减少重复和中文表达，使文本更正式、自然、凝练、易读，并降低 AI 润色痕迹。

最终输出：
1. 最终润色版；
2. 主要修改说明；
3. 仍需作者确认的问题。
## 十九、最终通篇检查 Prompt
### 适合投稿前最后一轮。
请作为 <你想投的期刊> 的英文论文语言编辑，对下面全文进行最终通篇检查。

检查重点：
1. 标题、摘要、引言、文献综述、方法、结果、讨论、结论之间的逻辑是否一致；
2. 术语是否统一；
3. 是否存在中式英语、口语化表达和不自然搭配；
4. 是否存在 AI 润色痕迹较重的句子；
5. 是否有重复过多的词或句式；
6. 是否有明显语法、拼写、标题错误；
7. 政策含义是否有结果支撑；
8. 是否有过度泛化或结论超出数据的问题。

请输出：
A. 修改后的全文；
B. 用列表说明关键修改；
C. 标出仍需作者核对的数据、引用或公式。
## 二十、带高亮修改 Prompt
### 如果你要生成 Word 高亮版，可以用这个。
请在原文基础上进行润色，并将所有明显修改、新增或重写的内容用黄色高亮标出。

要求：
1. 小的语法修正可以不高亮；
2. 逻辑重组、句子重写、术语替换、段落新增需要高亮；
3. 不改变数据、引用、公式和图表编号；
4. 保留原有标题层级；
5. 输出可用于 Word 文档的版本。
