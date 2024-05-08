+++
title = 'Med Eval测评结果'
date = 2024-01-03T18:14:28+08:00
draft = true
+++

## Med-Eval-Chinese Doctor

| **模型**           | **基座**           | **数据**                                                     | **得分**             |
| ------------------ | ------------------ | ------------------------------------------------------------ | -------------------- |
| Doctor             | Baichuan2-13B-Chat | 2.23125GB PT数据集epoch=1.0,loss=2.1348 <br />60.06MB SFT数据epoch=2.5，loss~2.00 | 32.22% 31.82% 31.86% |
| AiMed              | Baichuan2-13B-Chat | 215.3MB PT数据集 epoch=1.0,loss=2.332  <br />48.03MB SFT数据epoch=4.0,loss~1.900 | 23.43% 23.79% 23.40% |
| Baichuan2-13B-Chat | -                  | -                                                            | 13.64% 13.57% 13.53% |

带有prompt工程后：

| 指标                   | 指标含义       | Doctor | AiMed  |
| ---------------------- | -------------- | ------ | ------ |
| total_questions        | 总问题数       | 2773   | 2773   |
| strict_correct_answers | 严格得分       | 1087   | 786    |
| Model Strict Accuracy  | 严格得分率     | 39.20% | 28.34% |
| loose_correct_answers  | 绝对宽松得分   | 1583   | 1107   |
| Model Loose Accuracy   | 绝对宽松得分率 | 57.09% | 39.92% |
| loose_correct_answers2 | 相对宽松得分   | 1594   | 1177   |
| Model Loose Accuracy2  | 相对宽松得分率 | 57.48% | 42.45% |
| error_answers          | 错误           | 1179   | 1596   |
| Model Error            | 错误率         | 42.52% | 57.55% |
