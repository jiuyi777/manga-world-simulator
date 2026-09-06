# 漫画世界模拟器

漫画世界模拟器独立前端的 Android 与 Windows 公开测试包。无需安装 SillyTavern。

## 下载

前往 [Releases 下载页面](https://github.com/jiuyi777/manga-world-simulator/releases) 获取 APK 或 Windows ZIP。不要下载 GitHub 自动生成的 Source code ZIP 来安装软件。

- Android：下载 APK，支持 Android 8.0 及以上。
- Windows：下载 Windows-x64 ZIP，完整解压后双击 `漫画世界模拟器.exe`。其他文件也是运行必需的，不能只取出 EXE。支持 Windows 10/11 64 位。

## 使用

在“接口”里配置自己的模型服务。主剧情接口与额外变量解析接口可以分别设置，两边均支持拉取模型列表，也可以手填模型 ID。生成剧情需要可用的模型服务；安装包不包含接口密钥。

预设支持导入、条目开关、拖动排序、复制粘贴、删除及生成参数。提供世界书编辑、存档导入导出、单轮摘要、上下文查看与关键词搜索、跳转楼层。默认发送最近五层正文，可自行调整。

在尚未发送玩家行动的开场阶段，可以 Roll 开场白。玩家输入“大总结”并成功完成后，会用总摘要替代当前档此前逐轮历史，保留当前变量继续；失败不清空旧历史。重要剧情请先另存或导出备份。

各平台数据独立，不会自动同步。可用存档导出/导入迁移，接口信息需要另外填写。更新前请导出重要存档。

## 测试与限制

当前为公开测试版，非稳定发行：

- 已完成隔离浏览器、本地模拟接口以及打包 Windows 程序的相关功能测试。
- APK 使用 Android 测试证书；Windows 程序未做商业代码签名。请核对下载来源和 Release 中的 SHA-256；不需要关闭系统防护。
- 尚未完成实体 Android 设备和用户真实模型接口验收；供应商对模型列表、生成参数的支持可能不同。
- 兼容部分酒馆预设结构，并非完整 SillyTavern 运行环境；复杂宏、EJS 与插件脚本不保证兼容。

此仓库目前用于交付包和使用说明，不包含完整开发源码、用户存档或密钥。Windows 包随附 Electron 的 LICENSE 与 LICENSES.chromium.html。立绘与背景目录见 [manga-world-npc-portraits](https://github.com/jiuyi777/manga-world-npc-portraits)；未额外授予第三方素材的授权。
