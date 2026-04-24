+++
date = '2026-04-24T07:57:30+08:00'
draft = false
title = '下载'
+++

以下提供 Bookworm 最新稳定版的下载渠道，由[NVDA中文站](https://www.nvdacn.com/)提供资源下载支持。

**安装版（Setup）和便携版（Portable）分别适用于长期稳定使用和灵活移动场景。其中，x64版本专为64位系统设计，性能更优；x86版本则适用于32位系统。Bookworm基于Python 3.10开发，仅兼容Windows 8.1及以上操作系统。**

### 从中文站下载稳定版：

[Bookworm-2026.1-x64-setup](https://dl.nvdacn.com/Share/Bookworm/Stable/Bookworm-2026.1-x64-setup.exe)

[Bookworm-2026.1-x64-portable](https://dl.nvdacn.com/Share/Bookworm/Stable/Bookworm-2026.1-x64-portable.zip)

[Bookworm-2026.1-x86-setup](https://dl.nvdacn.com/Share/Bookworm/Stable/Bookworm-2026.1-x86-setup.exe)

[Bookworm-2026.1-x86-portable](https://dl.nvdacn.com/Share/Bookworm/Stable/Bookworm-2026.1-x86-portable.zip)



## 更新内容

### 本地化更新
* **西班牙语**：添加了西班牙语翻译（[@ericdq](https://github.com/ericdq)，[#283](https://github.com/blindpandas/bookworm/pull/283)）
* **芬兰语**：更新了翻译、文档及用户指南（[@jkinnunen](https://github.com/jkinnunen)，[#284](https://github.com/blindpandas/bookworm/pull/284), [#316](https://github.com/blindpandas/bookworm/pull/316), [#342](https://github.com/blindpandas/bookworm/pull/342)）
* **简体中文**：更新了文档及界面翻译（[@cary-rowen](https://github.com/cary-rowen)，[#293](https://github.com/blindpandas/bookworm/pull/293), [#369](https://github.com/blindpandas/bookworm/pull/369)）
* **葡萄牙语**：翻译更新（[@George-br](https://github.com/George-br)，[#296](https://github.com/blindpandas/bookworm/pull/296)）
* **法语**：翻译更新（[@sofquipeut](https://github.com/sofquipeut)，[#313](https://github.com/blindpandas/bookworm/pull/313)）
* **格鲁吉亚语**：翻译更新（[@DraganRatkovich](https://github.com/DraganRatkovich)，[#368](https://github.com/blindpandas/bookworm/pull/368)）

### 功能与增强
* 添加了百度在线 OCR 引擎（[@cary-rowen](https://github.com/cary-rowen)，[#334](https://github.com/blindpandas/bookworm/pull/334)）
* 添加了由 NVDACN 授权的 Vivo OCR 引擎（[@cary-rowen](https://github.com/cary-rowen)，[#338](https://github.com/blindpandas/bookworm/pull/338)）
* 为 TTS 实现了全局和本地媒体键控制（[@cary-rowen](https://github.com/cary-rowen)，[#328](https://github.com/blindpandas/bookworm/pull/328)）
* 在用户界面中添加了文本折行选项（[@cary-rowen](https://github.com/cary-rowen)，[#299](https://github.com/blindpandas/bookworm/pull/299)）
* 增加了按位置对书签进行排序的功能（[@pauliyobo](https://github.com/pauliyobo)，[#324](https://github.com/blindpandas/bookworm/pull/324)）
* 允许从 QRD 文件导入书籍元数据（[@pauliyobo](https://github.com/pauliyobo)，[#310](https://github.com/blindpandas/bookworm/pull/310)）
* 增加了“查看升级日志”的菜单项（[@cary-rowen](https://github.com/cary-rowen)，[#337](https://github.com/blindpandas/bookworm/pull/337)）

### 文档处理
* 每当 EPUB 或 Word 文件被修改时，自动更新文档缓存（[@pauliyobo](https://github.com/pauliyobo)，[#289](https://github.com/blindpandas/bookworm/pull/289)）
* 修复了导致 .docx 文档无法打开的错误（[@pauliyobo](https://github.com/pauliyobo)，[#312](https://github.com/blindpandas/bookworm/pull/312), [#315](https://github.com/blindpandas/bookworm/pull/315)）
* 保留原始 URI，以确保转换后的文档能正确恢复上次阅读位置（[@cary-rowen](https://github.com/cary-rowen)，[#340](https://github.com/blindpandas/bookworm/pull/340)）
* **EPUB 特定修复**：
    * 处理了 EPUB HTML 片段中缺失 `<head>` 或 `<body>` 标签的情况（[@cary-rowen](https://github.com/cary-rowen)，[#319](https://github.com/blindpandas/bookworm/pull/319)）
    * 修复了 EPUB 中非标准布局的表格导航问题（[@cary-rowen](https://github.com/cary-rowen)，[#362](https://github.com/blindpandas/bookworm/pull/362)）
    * 针对格式错误的 HTML 内容在 `_get_title_for_section` 中增加了异常处理（[@cary-rowen](https://github.com/cary-rowen)，[#356](https://github.com/blindpandas/bookworm/pull/356)）
    * 修正了 `get_epub_html_item_by_href` 中的拼写错误（[@cary-rowen](https://github.com/cary-rowen)，[#357](https://github.com/blindpandas/bookworm/pull/357)）

### 导航与注释
* 支持针对行内的特定部分添加注释（[@pauliyobo](https://github.com/pauliyobo)，[#280](https://github.com/blindpandas/bookworm/pull/280)）
* 修复了注释导航错误，并改进了基于点的注释行为（[@cary-rowen](https://github.com/cary-rowen)，[#336](https://github.com/blindpandas/bookworm/pull/336)）
* 修复了更改存储路径后导致文档丢失关联注释的问题（[@pauliyobo](https://github.com/pauliyobo), [@cary-rowen](https://github.com/cary-rowen)，[#349](https://github.com/blindpandas/bookworm/pull/349)）
* 解决了链接文本显示不全及脚注导航问题，并调整了光标位置（[@cary-rowen](https://github.com/cary-rowen)，[#318](https://github.com/blindpandas/bookworm/pull/318), [#320](https://github.com/blindpandas/bookworm/pull/320), [#322](https://github.com/blindpandas/bookworm/pull/322)）

### 通用修复与改进
* 为更新检查实现了更好的版本比较逻辑（[@cary-rowen](https://github.com/cary-rowen)，[#301](https://github.com/blindpandas/bookworm/pull/301)）
* 加强了语音引擎的加载稳定性，并解决了配置不匹配的问题（[@cary-rowen](https://github.com/cary-rowen)，[#339](https://github.com/blindpandas/bookworm/pull/339)）
* 为 `http_resource` 请求添加了 User-Agent（[@pauliyobo](https://github.com/pauliyobo)，[#347](https://github.com/blindpandas/bookworm/pull/347)）
* 使用特定的 `TextFixerConfig` 实例来控制 ftfy 的文本修正过程（[@cary-rowen](https://github.com/cary-rowen)，[#298](https://github.com/blindpandas/bookworm/pull/298)）
* 交换了阅读器工具栏中缩放按钮的标签以使其更清晰（[@cary-rowen](https://github.com/cary-rowen)，[#292](https://github.com/blindpandas/bookworm/pull/292)）

### 依赖与工具更新
* **构建与环境**：
    * 迁移至 uv/ruff，并改进了构建系统及环境元数据（[@cary-rowen](https://github.com/cary-rowen)，[#351](https://github.com/blindpandas/bookworm/pull/351), [#352](https://github.com/blindpandas/bookworm/pull/352)）
    * 添加了 pytest 的 CI 工作流（[@cary-rowen](https://github.com/cary-rowen)，[#355](https://github.com/blindpandas/bookworm/pull/355)）
    * 添加了 Winget 自动发布工作流（[@cary-rowen](https://github.com/cary-rowen)，[#359](https://github.com/blindpandas/bookworm/pull/359)）
    * 配置了 Dependabot 以实现自动更新（[@cary-rowen](https://github.com/cary-rowen)，[#360](https://github.com/blindpandas/bookworm/pull/360)）
* **依赖库升级**：
    * 升级了多项依赖以解决弃用警告（[@cary-rowen](https://github.com/cary-rowen)，[#358](https://github.com/blindpandas/bookworm/pull/358)）
    * 将 `urllib3` 升级至 2.6.3（[@dependabot](https://github.com/dependabot), [@cary-rowen](https://github.com/cary-rowen)，[#345](https://github.com/blindpandas/bookworm/pull/345), [#350](https://github.com/blindpandas/bookworm/pull/350), [#353](https://github.com/blindpandas/bookworm/pull/353), [#354](https://github.com/blindpandas/bookworm/pull/354)）
    * 将 `jinja2` 升级至 3.1.6（[@dependabot](https://github.com/dependabot)，[#291](https://github.com/blindpandas/bookworm/pull/291), [#308](https://github.com/blindpandas/bookworm/pull/308)）
    * 将 `requests` 从 2.32.3 升级至 2.32.4（[@dependabot](https://github.com/dependabot)，[#325](https://github.com/blindpandas/bookworm/pull/325)）
    * 将 `mammoth` 从 1.7.1 升级至 1.11.0（[@dependabot](https://github.com/dependabot)，[#344](https://github.com/blindpandas/bookworm/pull/344)）
    * 升级了 actions 组插件（[@dependabot](https://github.com/dependabot)，[#361](https://github.com/blindpandas/bookworm/pull/361), [#365](https://github.com/blindpandas/bookworm/pull/365)）

---

## 新贡献者
* [@ericdq](https://github.com/ericdq) （[#283](https://github.com/blindpandas/bookworm/pull/283)）
* [@George-br](https://github.com/George-br) （[#296](https://github.com/blindpandas/bookworm/pull/296)）
* [@sofquipeut](https://github.com/sofquipeut) （[#313](https://github.com/blindpandas/bookworm/pull/313)）

**完整变更日志**: [2024.2...2026.1](https://github.com/blindpandas/bookworm/compare/2024.2...2026.1)
