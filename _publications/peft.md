---
title: "Exploring parameter-efficient fine-tuning of large language model on automated program repair"
collection: publications
category: conferences
permalink: /publication/peft
date: 2024-10-27
venue: 'ASE 24: Proceedings of the 39th IEEE/ACM International Conference on Automated Software Engineering'
slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'http://academicpages.github.io/files/paper1.pdf'
citation: 'Li, Guochang, et al. "Exploring parameter-efficient fine-tuning of large language model on automated program repair." Proceedings of the 39th IEEE/ACM International Conference on Automated Software Engineering. 2024.'
---

Automated Program Repair (APR) aims to fix bugs by generating patches. And existing work has demonstrated that "pre-training and fine-tuning" paradigm enables Large Language Models (LLMs) improve fixing capabilities on APR. However, existing work mainly focuses on Full-Model Fine-Tuning (FMFT) for APR and limited research has been conducted on the execution-based evaluation of Parameter-Efficient Fine-Tuning (PEFT) for APR. Comparing to FMFT, PEFT can reduce computing resource consumption without compromising performance and has been widely adopted to other software engineering tasks.
To fill this gap, we enhance the existing APR dataset by employing prompt engineering to create an instruction dataset, APR-INSTRUCTION, at first. Secondly, we fine-tune four pre-trained LLMs using four different PEFT methods with APR-INSTRUCTION. The best fine-tuned model fixes 58% more bugs than the state-of-the-art LLM-based APR techniques. The results also show that $(IA)^3$ improves the creativity of LLMs more effectively through fine-tuning and achieves the highest fixing capability compared to the other three PEFT methods. Thirdly, we explore the optimal configuration of PEFT hyperparameters, and assess the impact of instruction dataset size, showing that a larger number of parameters and a larger training dataset do not necessarily result in better performance for PEFT. Lastly, we analyze peak memory usage and trainable parameters to show the efficiency of PEFT.
This work provides a comprehensive exploration of PEFT on APR and suggests potentially promising directions for extension to other software engineering downstream tasks. APR-INSTRUCTION, PEFT weights, and the fine-tuning code are publicly available as open-source resources.