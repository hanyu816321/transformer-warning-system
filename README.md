<img width="1503" height="576" alt="image" src="https://github.com/user-attachments/assets/f0b8dadf-c72c-4193-b07b-9e4bbfce48a5" />


v2/
├── BE/                       后端(FastAPI,算法层与 Web/DB 解耦)
│   ├── app/
│   │   ├── api/              路由:detect / diagnose / trend / warning / decision / dataset / agent / assistant
│   │   ├── algorithms/       纯算法(输入输出 DataFrame,不依赖 DB/HTTP)
│   │   │   ├── detect/       表A.3 四档分级 + §9.3.3 处置紧急度(不改档位)
│   │   │   ├── diagnose/     特征气体 + 三比值 + Duval + 交叉研判/试验映射
│   │   │   ├── agent/        工作流+工具+决策轨迹+运行日志展开+B 报告(LLM/模板)+表G.1/G.2+报告导出
│   │   │   ├── assistant/    分析助手：意图/规则解释/FAQ/润色/会话 sync（不改七步内核）
│   │   │   ├── knowledge/    判据条目 refs(角标依据,非 RAG)
│   │   │   └── synthesis.py  合成时序(单台×360天)
│   │   ├── core/ / db/ / main.py
│   │   └── .env.example      LLM 可选配置
│   └── scripts/
├── FE/                       前端(Vue3)
│   └── src/views/            数据集 / 分级 / 趋势 / 告警 / 决策 / 判型 / Agent / 知识库
├── docs/                     decisions-log / 项目总结 / 论文章节骨架
└── data/

<img width="1488" height="678" alt="image" src="https://github.com/user-attachments/assets/3c8d5672-58b0-4a59-84a1-c1b160ba11dd" />

<img width="1482" height="780" alt="image" src="https://github.com/user-attachments/assets/9f052848-8adc-436a-be82-f88e3744a1ea" />

<img width="1449" height="279" alt="image" src="https://github.com/user-attachments/assets/2fb1ed77-53dd-4ed7-8358-d44c129f7475" />

<img width="1524" height="780" alt="image" src="https://github.com/user-attachments/assets/ce2064e5-1fd7-4efb-a5ed-c19426d93662" />

<img width="1449" height="714" alt="image" src="https://github.com/user-attachments/assets/6f5bd98a-49dd-4bc0-888f-9466f48421e2" />

<img width="1434" height="510" alt="image" src="https://github.com/user-attachments/assets/07a88c7d-613d-4ff8-95e2-d7c93757ce0a" />
