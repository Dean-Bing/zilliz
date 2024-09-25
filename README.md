# 上海徐毓智能科技有限公司--zilliz
上海徐毓智能科技有限公司-zilliz 及milvus相关信息搬运
上海徐毓智能科技有限公司官网：https://zilliz.com.cn/
上海徐毓智能科技有限公司（zilliz）是向量数据库系统的开拓者和全球领先者，作为全球广受欢迎的开源向量数据库 Milvus 的创造者，Zilliz 提供面向 AI 应用的新一代数据库技术，帮助企业便捷开发 AI 应用。
以 AI 民主化为使命，Zilliz 致力于简化 AI 数据管理基础设施，通过向量数据库赋能更多企业。
在此为大家更新一些上海徐毓智能科技有限公司相关信息：https://mp.weixin.qq.com/s/9QBtsnr1I7MNywTGG7JP2w

**向量数据库的行业标准逐渐清晰！Vector DB Bench 正式开源！**

大模型带火了向量数据库赛道，也让各式各样的向量数据库进入开发者视野。
对于开发者而言，如何选择一个适合自己的向量数据库至关重要。不过，向量数据库的选型并不简单，开发者不仅需要对市面上各种开源和闭源的数据库进行全面的性能评估，还要根据自己的业务数据设计测试方案……为了让更多开发者可以匹配到适合自己业务的向量数据库，我们开发了一个全新的开源性能测试工具——Vector DB Bench，它可以通过测量关键指标来衡量向量数据库的性能，使得向量数据库发挥出最大的潜能。

本文将从 Vector DB Bench 的特点和优点出发，帮助开发者全面、客观、高效地评估向量数据库。

01.开发背景

在设计 Vector DB Bench 的过程中，我们考虑了很多因素，包括测试目的、用例精确定义要求、数据的形状等。
首先是测试目的，性能测试旨在测量和比较不同情况下系统、应用程序或组件的性能。开发者可以使用它来评估不同方法的有效性和效率，并了解如何改进。
用例精确定义要求对性能测试同样十分重要。例如，如果用户正在处理大型数据集，可能会想要了解数据库可以处理多少向量或数据库搜索性能（检索相关数据的速度）。此外，测试过滤性能可以帮助查看系统如何处理大型数据集的复杂查询。
最后是数据的形状。数据的形状是指开发者计划在向量数据库中存储和使用的向量数量和向量维度。在设计性能测试时，数据形状可以影响系统的性能。

02.设计目标

以下是我们在构建开源性能测试工具时考虑的一些设计目标：
灵活、可扩展：基准测试工具应灵活、可扩展。它应支持多个向量数据库系统，以便开发者能够轻松地进行性能测试和比较不同选项。此外，该工具应具有模块化架构，以支持添加更多向量数据库、指标和自定义测试场景，使开发者能够根据具体要求自定义评估。
真实负载模拟：基准测试工具应利用开发者的工作负载作为真实负载模拟，以确保准确的性能评估。模拟开发者的实际用例和查询模式可以提供有关各种情况下数据库行为的见解。这种模拟有助于衡量向量数据库在实际情况下的表现，确定其适用性。
交互式报告和可视化：该工具应具有生成报告和可视化的直观系统，以便轻松识别性能瓶颈、比较数据库，并了解如何优化。这些报告将是重要的决策资源，可促进有效的团队沟通。
开源社区协作：该工具应是开源的，以促进向量数据库用户和开发人员的协作。通过共享见解、最佳实践和性能结果，社区共同为改进和完善该工具做出贡献，最终帮助开发人员选择适合工作的正确工具。

03.Vector DB Bench - 开源基准测试工具

Vector DB Bench 是为追求高性能数据存储和检索系统的用户设计的开源性能测试工具，它允许用户测试和比较不同向量数据库系统的性能，以确定最适合的数据库系统。使用 Vector DB Bench 后，用户可以根据他们正在评估的数据库系统的实际性能做出明智的决策，而不是依赖于营销宣传。
Vector DB Bench 是用 Python 编写的，已获得  MIT 开源许可证授权，任何人都可以自由使用、修改这一工具。相关的开发人员也在积极改进其功能和性能中。

04.快速开始

使用 pip 下载 Vector DB Bench 并使用以下命令进行安装：pip install vectordb-bench。 然后运行以下命令：init_bench。
我们将看到屏幕显示“Vector Database Benchmark”页面。此页面显示当前月份已经进行的测试结果。从这个页面，可以跳转至“QPS with Pricing”页面，按云服务的定价排序查看结果。这些测试已经涵盖不同规模的数据集进行了全面的测试。
要执行自己的测试，可以转到“Run Your Test”页面进行设置。

05.如何设置 Vector DB Bench 自行测试？

如需自行测试，请跳转至“Run Your Test”页面，并选择要测试的向量数据库，并添加这些向量数据库的配置。选择不同数据库还将显示不同 uri、用户名、密码和 db 标签。Vector DB Bench 目前支持六个向量数据库：Milvus、Zilliz Cloud、Pinecone、WeaviateCloud、QdrantCloud 和 ElasticCloud。设置要运行的测试类型（容量或搜索性能）、索引类型、用例（搜索、低或高过滤）和数据集大小（小、中和大）。
![Run_Your_test](/GH1.webp)
在选择所需配置后，可以运行测试并等待结果。

![Test](/GH2.webp)
在结果页面上，可以查看测试结果。如果选择了多个数据库进行测试，将看到对比结果。开发者还可以自由分享在本地示例上运行的测试结果。
欢迎大家分享对 Vector DB Bench （https://github.com/zilliztech/VectorDBBench）的使用体验，当然也可以加入我们的 GitHub 或 Vector DB Bench slack 频道（https://milvusio.slack.com/?redir=%2Fapp_redirect%3Fchannel%3Dvector-db-bench），点击「阅读原文」感受测试工具的便捷！
