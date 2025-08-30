# KART 汉化工具

自动扫描并修改 Kaspersky Anti-Ransomware Tool 的界面资源，实现中文界面。

## 功能特点
- 正常模式启动后提示重启到安全模式
- 安全模式下自动备份并替换语言 JSON
- 完成后移除 SafeBoot 设置并重启回正常模式
- 使用 PyQt5 提供现代化对话框

## 运行要求
- Python 3.8+
- Windows 系统，需管理员权限
- [PyQt5](https://pypi.org/project/PyQt5/)

## 使用方法
1. 安装依赖：`pip install PyQt5`
2. 在正常模式下以管理员身份运行 `python kart汉化.py`
3. 根据提示重启进入安全模式，脚本会自动完成汉化并重启回正常模式

## 打包
使用 [PyInstaller](https://pyinstaller.org/) 并配合仓库内的 `kart汉化.spec` 打包可执行文件：

```bash
pyinstaller kart汉化.spec
```

## 授权协议
本项目基于 [GNU General Public License v3](LICENSE) 发布。
