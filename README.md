# MacInspector 社区模块库

MacInspector 菜单栏监控工具的社区模块配置库。

## 仓库结构

```
index.json         模块清单（软件拉取此文件）
modules/*.json     每个模块一个 .minsp 包（软件内导出的格式）
```

## 使用

在 MacInspector 设置窗口 → Community Library 填入本仓库地址：
`https://github.com/Zekilou/macinspector-modules`

## 贡献模块

1. 在软件内编辑好模块，右键 → Export .minsp...
2. 把导出文件放进 `modules/`，文件名用模块 id（如 `cpu.json`）
3. 在 `index.json` 的 `modules` 数组加一条记录：

```json
{ "id": "cpu", "name": "CPU 监控", "description": "简介", "file": "modules/cpu.json", "author": "你的名字", "tags": ["cpu"] }
```

4. 提 PR 即可
