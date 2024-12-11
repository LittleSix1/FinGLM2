# FinGLM

## 仓库介绍

本仓库是关于 [2024金融行业·大模型挑战赛](https://competitions.zhipuai.cn/matchDetail?id=120241202000000003) 的开源代码汇总，
旨在探索大语言模型在法律行业的应用潜力。 本仓库存放了数个比赛团队的竞赛原始代码，均经过整理并开源。

## 项目更新

- **News**: ```2024/12/11```:  本仓库关于BaseLine提交要求和例子提供。

## BaseLine 提交说明

### 评测化境说明

- Python 3.12.7 / Python 3.10.13
- Ubuntu 22.04 操作系统, 不提供 GPU / NPU，仅保证`UTF-8`编码格式能正常解码。
- 仅能访问智谱AI API，pip清华源仓库, 比赛数据库, 不提供联网服务。评测环境提供智谱AI API KEY，但不具备联网功能。
  > 如果你提交的代码依赖源码安装的pip包，请在README中写明，主办方将从github拉取对应pip包主分支。

### 提交规范

- 不允许提交`csv, txt, json, yaml, xlsx`等格式本地硬编码文件，不允许提交`.idea, .DS_Store`
  等无效文件和本地缓存文件。本仓库会提供比赛的参考材料，放置在[assets](assests),
  所有的预处理工作必须基于这些材料进行，不能使用比赛之外的材料。所有的操作都必须通过大模型和比赛材料运行和操作。
- 提交代码文件请使用`ruff`格式刷。确保满足`PEP 8`规范。规范文件请参考这里: [规范文件](pyproject.toml)
- 不能在一个大模型对话中联系提问一套问题的三个小问题。
- 必须提交一个`README.md`用以解释你的思路，确保复现人员能够理解你的代码, 以及根据`requirements.txt`来安装依赖。若运行失败，则提交无效。
- 必须提交一个`jupyter notebook`文件，用以展示你的代码运行结果。确保代码能够正常运行，否则提交无效。
- 所有`API_KEY`必须用环境变量，或者外部传递变量的方式传递。
- 请不要直接贡献到这个仓库，而是通过比赛链接上传到比赛官方进行评测。不满足提交规范的作品将不被收录。你可以参考 [例子](baseline/sample/README.md)。

## 开源协议

本代码中无特殊说明或者无注名额外协议的，均使用 [Apache 2.0](LICENSE) 协议。
