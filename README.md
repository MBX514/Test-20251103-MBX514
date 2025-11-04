# 大模型专家测试项目

仓库: `Test-20251103-MBX514`  
作者: MBX514  
完成时间: 2025年11月

项目概述

本项目完成了大模型专家测试的所有题目，包含三个独立模块：

A卷 · 多选题 (40分)
- 20道专业选择题，涵盖Python、数据库、Docker等领域

B卷 · 编程题 (45分)
- B1: 数据清洗脚本 (15分)
- B2: 最小待办REST API (20分)  
- B3: Docker & CI/CD配置 (10分)

C卷 · 问答题 (15分)
- 5道综合问答题，考察系统设计能力

项目结构
Test-20251103-MBX514/
├── 1ACS/ # B1题 - 数据清洗
│ ├── scripts/
│ │ └── clean_orders.py # 数据清洗脚本
│ ├── tests/
│ │ └── test_clean.py # 数据清洗测试
│ ├── data/
│ │ └── orders_raw.csv # 样例数据
│ └── requirements.txt # Python依赖
├── 2ACS/ # B2题 - REST API
│ ├── app/
│ │ ├── main.py # FastAPI应用
│ │ ├── db.py # 数据库配置
│ │ ├── models.py # 数据模型
│ │ ├── schemas.py # Pydantic模式
│ │ └── crud.py # 数据库操作
│ ├── tests/
│ │ └── test_api.py # API测试
│ └── requirements.txt # Python依赖
├── 3ACS/ # B3题
│ ├── app/ # FastAPI应用（同2ACS）
│ ├── tests/ # 测试用例
│ ├── .github/workflows/ # CI/CD配置
│ ├── Dockerfile # 容器化配置
│ ├── docker-compose.yml # 服务编排
│ ├── validate_setup.py # 配置验证脚本
│ └── requirements.txt # Python依赖
├── .github/workflows/ # 根目录CI工作流
├── .gitignore # Git忽略规则
└── README.md # 项目说明
