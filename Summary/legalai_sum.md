# Study

## LAiW: A Chinese Legal Large Language Models Benchmark

**问题**：现有的LLM in LegalAI的评估方法与legal Logic（legal syllogism）不一致，导致一些不可信的问题，难以在现实场景利用。legal logic 指的是三段论（legal syllogism）：Major Premise、Minor Premise、Conclusion （Legal Article、evidence of a case,  judicial decision）。

**方案**：为了解决这个问题，本研究构造了一个Legal LLMs BenchMarks-**LAiW**，将法律任务分为三类：basic information retrieval （BIR）, legal foundation inference （LFI）, complex legal application (CLA)，分别测试LLMs在三类任务上的能力。BIR检测了LLM在对于Major Premise 和 Minor Premise 的抽取能力；LFI任务形式相对简单，测试了LLM利用大前提和小前提的推理能力；CLA测试了模型的在复杂法律任务上的能力。

**结论**：LLM可能学习到了生成法律文本的模式，但是对于法律逻辑的利用的能力较差。

**疑问**：文章的出发点很好贴合实际场景，但是有几个疑问：

1. 文章说LLM在CLA上的表现比LFI任务高20个点，两个任务的评价标准不一样，怎么比的。
2. 作者得出结论LLM对legal syllogism的利用能力不足，但是设计的提示模板不是三段论的形式，如何说明LLM对legal syllogism的利用能力不足？

**感觉实验不足以支撑其主张**。