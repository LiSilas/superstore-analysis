项目简介：
这是一个基于 Superstore 商业交易数据的分析与预测项目，目标是帮助企业洞察销售规律、预测未来趋势、识别高价值客户并优化业务策略。
本项目不仅适合商业数据分析岗候选人展示数据处理与建模能力，也可作为零售、电商等行业的数据驱动决策工具原型。

项目价值与功能：
- 销售趋势洞察：分析不同时间、地区、产品类别的销售和利润结构，帮助企业发现增长点与亏损源。
- 未来销售预测：基于历史数据预测未来 12 个月销售额变化，支持库存与生产计划优化。
- 亏损订单识别：提前标记潜在亏损订单，降低经营风险。
- 客户价值分群（RFM 模型）：将客户分为高、中、低价值群体，用于精准营销与会员管理。
- 可视化展示：用 Python 和 Power BI 输出可视化报表，直观呈现业务现状与趋势。

项目结构：
superstore-analysis/
├── datasets/                     # 数据集（需自行下载）
├── sales_model.pkl                # 销售预测模型
├── loss_model.pkl                 # 亏损预测模型
├── main.py                        # 主程序（数据处理+分析+建模）
├── requirements.txt               # 依赖列表
├── README.md                      # 项目说明
├── output/
│   ├── sales_predictions.csv       # 销售预测结果
│   ├── loss_predictions.csv        # 亏损预测结果
│   ├── monthly_sales_forecast.csv  # 时间序列预测结果
│   └── customer_clusters.csv       # 客户分群结果


数据集不包含在仓库中，请自行下载 Superstore 数据并放入 datasets/ 目录。（https://www.kaggle.com/datasets/vivek468/superstore-dataset-final）
注意：项目中的训练模型较大（400MB+），未包含在仓库中。如需使用模型，请自行运行代码生成。

工作流程：
1.数据预处理：缺失值处理、时间字段拆解、特征编码、数值特征保留
2.探索性分析（EDA）：销售趋势、利润分布、折扣与利润关系、热力图、Top 客户分析
建模与预测
3.回归模型：预测订单销售额（Random Forest Regressor）
4.分类模型：识别亏损订单（Random Forest Classifier）
5.时间序列预测：Prophet 模型预测未来销售趋势
6.客户分群：基于 RFM 指标的高/中/低价值客户分类
7.可视化输出：Matplotlib、Seaborn 及 Power BI 报表

技术栈：
- 数据分析：Python、pandas、numpy
- 可视化：matplotlib、seaborn、Power BI
- 机器学习：scikit-learn、prophet
- 模型管理：joblib
- 客户分析：RFM 模型、KMeans 聚类

适用场景：
- 企业销售数据分析与季度汇报
- 电商平台的会员分群与营销策略优化
- 零售行业的库存与生产计划预测

- 数据分析岗、商业智能岗面试作品集展示
