> **0.3.2 国家图书馆三款时装模型已发布：** [下载本版增量更新](https://github.com/Mizusamada/TerraDeskMateStandard/releases/tag/v0.3.2-standard)。先安装原 0.3.1，再按 [更新说明](docs/RELEASE-0.3.2.md) 操作；旧 EXE 不自动包含新皮肤。

<!-- BEGIN DOWNLOAD FRONT -->
# ⬇ 普通用户：下载即用

**[直接下载 标准版 0.3.1 EXE](https://github.com/Mizusamada/TerraDeskMateStandard/releases/download/v0.3.1-standard/TerraDeskMateStandard-OneClick-Setup-0.3.1.exe)** · **[安装/便携使用说明](00-下载安装/README.md)** · **[按角色下载](00-下载安装/角色下载目录.md)**

单个联网安装 EXE 自动下载所有分卷并更新，无需手动打补丁。普通用户不需要 Node.js/npm；下方源码说明面向开发者。

<!-- END DOWNLOAD FRONT -->

## 0.3.1 角色与稳定性更新

最新资源：434角色、2853模型；新增克莱门莎、德·托莱多、旅骨，及酒神/真言/烈夏三套错位巡礼皮肤。新角色中日官方原声已补齐，日文原文标注仍缺，不能作为已审阅训练稿。Light通过六个完整角色包导入新增内容，其余版保留内置全角色。详见 `docs/RELEASE-0.3.1.md`。本次Release是0.3.0基础上的增量补丁，不是首次安装包；旧完整安装器和便携包保留。

# TerraDeskMateStandard · 泰拉桌伴标准版

Windows x64，0.3.0。保留431角色/2835模型、动作/皮肤/原声/台词/档案。**不含41套专属语音训练权重，不含内置Python、Torch、GPT-SoVITS环境与通用模型**。原声是已有录音，不依赖Python；AI文字聊天需要另配LLM服务。本地AI语音须自行安装或连接外部完整GPT-SoVITS环境。

## 普通用户下载
从[Release](https://github.com/Mizusamada/TerraDeskMateStandard/releases)选：
- 安装版：下载TerraDeskMateStandard-Setup-0.3.0.exe和全部同名BIN到同一目录，双击EXE。
- 便携版：完整下载所有TerraDeskMateStandard-0.3.0-win-x64.7z.00N分卷，用7-Zip打开001解压完整目录，双击TerraDeskMate.exe。

显示、动作、原声不需要npm、系统Python或云端密钥。启动只打开控制中心，选择角色并点显示才出场。源码ZIP不是运行包。附件公开前保持草稿，不以源码上传代表运行包完整。

## 四版区别
|版本|角色基础资源|41套训练权重|内置Python/GPT-SoVITS|
|---|---|---|---|
|全量|全部|有，未全通过音色验收|有|
|Plus|全部|无|有|
|Standard|全部|无|**无**|
|Light|阿米娅及通用敌人，其他按需导入|本体无|无|

## 文档
[详细教程及注意事项](docs/Standard详细教程.md) · [分类手册](docs/使用说明书/00-目录.md)

## 开发者
仓库提供apps/services/packages/scripts源码。资源不直接提交Git，使用准备资源.ps1恢复基础资源，再npm ci、npm run build、npm start。Standard构建明确排除trained-voices与speech-runtime，不自动下载语音环境。程序保留用户自行配置外部语音服务的入口。

## 边界
安装器未签名，可能提示未知发布者。另一物理电脑、全部角色逐帧视觉和云端真人服务不宣称已验证。参考推理/训练/音频到音频变声是不同路线；Standard不附内置推理环境。
