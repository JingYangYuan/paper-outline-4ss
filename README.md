<p align="center">
  <img src="docs/banner.svg" alt="paper-outline-4ss" width="100%">
</p>

# Paper 论文大纲 4SS（outline 模块独立版）

将用户指定输入路径、master 输入登记表或当前目录候选材料转换为结构化论文撰写大纲。支持毕业论文（五章结构）和期刊论文（五要素紧凑结构）双轨输出，支持规范研究、实证研究、阐释研究、混合研究四种方法协议，以及社会学研究范式和管理世界案例研究范式两类发表风格。当用户需要从已有文献素材生成论文大纲、将材料转化为写作框架、或需要论文结构设计时使用。

本包由 `paper-master-4ss/scripts/export_standalone.py` 从总控包 `paper-master-4ss/modules/outline/` 自动导出：

- 包内相对路径相对本包根目录解析；
- `master/` 与 `references/` 中的协议/治理文件是导出时拷贝的快照；
- 跨模块路径 `paper-master-4ss/modules/<x>/...` 相对同级安装的总控包解析；
- 更新方式：修改总控包对应模块后运行
  `python3 paper-master-4ss/scripts/export_standalone.py outline` 重新导出，勿直接编辑本包。

## 它做什么

把已有文献素材转成可直接用于写作的结构化大纲：材料扫描 → 结构构建 → 段落级证据映射 → 缺口报告。支持毕业论文五章结构和期刊论文五要素紧凑结构。

## 双轨与协议

| 项 | 选项 |
|---|---|
| 输出轨道 | 毕业论文 / 期刊论文 |
| 方法协议 | 规范、实证、阐释、混合 |
| 发表风格 | 社会学研究范式 / 管理世界案例研究范式 |

## 使用

将本目录安装为宿主 skill（与 `paper-master-4ss` 总控包同级）。入口见 `SKILL.md`。
