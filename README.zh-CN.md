# Seifert 论文 Theorem 5.1：纸面核查

[English](README.md)

**结论：** 在“被引外部定理的完整陈述作黑箱、只核对适用条件；论文自己的推理采用已验收补法”的范围内，Theorem 5.1 的 (a)–(d) 成立。原稿需要更正。本次核查未证实重大漏洞。

## 对象与版本

对象为 Apex Intelligence 的 *Contractibility of the Complex of Incompressible Seifert Surfaces: The Knot Case of Kakimizu’s Problem*，日期 **2026 年 9 月 11 日**，官网比赛版 PDF，**Theorem 5.1（Incompressible exchange lemma），印刷第 13 页**。证明涉及 §5、§§3–4 的相关内容及附录 A–B。

- PDF 标识：`seifert-surfaces.pdf`。
- PDF SHA-256：`34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`。
- 本核查包：**v1.0，2026 年 10 月 4 日**。
- 仓库中的论文定位均使用**印刷页码**及定理、引理、章节或公式编号，不使用提取文本的本地行号。

PDF 哈希用于识别确切版本。本仓库不收录论文 PDF；后续版本新增的论证不回算为比赛版已有证明。

## 核查的陈述

设 $K$ 为非平凡结，$x,u,w$ 为 $IS(K)$ 的顶点，且

$$
\operatorname{dist}(x,u)=\operatorname{dist}(x,w)=1,
\qquad \operatorname{dist}(u,w)=2.
$$

以 $v\sim_{=}q$ 表示相等或邻接。存在在任何后来共同邻居 $z$ 给定前选定的 $w_\uparrow,w_\downarrow$，满足：

1. **(a)** 每个输出分别与 $x,u,w$ 相等或邻接。
2. **(b)** 任意分别与 $u,w$ 相等或邻接的 $z$，与两个输出分别相等或邻接。
3. **(c)** $g(w_\uparrow)+g(w_\downarrow)\le g(u)+g(w)$。
4. **(d)** 若 (c) 等号成立，则 $A(w_\uparrow)+A(w_\downarrow)<A(u)+A(w)$。

$A(v)$ 是光滑 neat 顶点类中、边界为固定纵向叶层之叶的曲面的相对面积下确界。核心顺序为 $\forall(x,u,w)\,\exists(w_\uparrow,w_\downarrow)\,\forall z$。不要求规范选择、唯一性或所有涉及的顶点同时具有不交代表。

## 范围与方法

这是离线结构化纸面核查，不是形式化证明证书。证明先经三路并行逐行核查，再由对抗复核尽力推翻其判定，并由跨模型抽查对照原文核实关键论断；对抗复核修正了某路结论的，以修正为准。本包汇总这些结果。

证明拆为 87 个输入或推理步骤，核对外部定理前件、光滑与分片光滑类别、局部椭圆论证、面积比较的合法竞争者、定量支撑和收益界，以及代表元、参数和压缩后代的选择顺序。局部反例模型针对特定推理，不宣称是 Theorem 5.1 的全局反例。

| 类型 | 数量 |
|---|---:|
| 引用外部成熟结果 | 16 |
| 论文论证或关键接口 | 51 |
| 标准事实或常规计算 | 20 |
| **总计** | **87** |

| 对原步骤的判定 | 数量 |
|---|---:|
| 成立 | 45 |
| 成立但需补法 | 37 |
| 存疑 | 3 |
| 在指定读法或应用下不成立 | 2 |

统计针对原拆分步骤。“成立”包括条件式推论与黑箱陈述适用性；修正版可用不等于原句已通过。

## 所需更正

- 将正文对 **Theorem A.6、Lemma A.7** 的调用改接 §3 已引用的完整 **E(ii)**：已核预印本的 Schultens Theorem 2／Kapovich 附录 Corollary 11，加**独立 Hopf 横截论证**。正文确实调用附录 A，这是一条替换路线，不能说原稿从未使用附录 A。
- **D29：** 不成立只限于真角端点的光滑环境同痕读法。角对象的拓扑运输用 tame 同痕；光滑同痕只比较两个正宽光滑端点。原稿另有分片光滑类别约定，不能将否定扩张到所有类别读法。
- **D28/D35：** 采用正光滑宽度、真实几何支撑界及四扇区共同数据；盘交换的光滑竞争面在**稍大光滑三球**中认证。
- **D43/D80/D81：** 同时缩圆角与推离尺度，比较正参数光滑族并运输**事前指定的压缩后代**，输出类先于 $z$ 固定。
- **D77–D79：** 只在有缓冲的好区取得统一数据；统一收益系数及全部宽度界，先定 $\varepsilon_*$，再选 $t$。
- 不可约性引用补 **[10, p. 228]**。其余分析、类别与引用精度更正见 [repairs.md](proof/repairs.md)。

## 限定与未闭合事项

**D09**（FHS 改编）与 **D10**（Kapovich 直接使用 Anderson Theorem 3.1，超过其截断曲面结论）限制对被引文献印刷证明的独立验收，不据此否定已发表陈述。**D12、D22** 使附录 A 的内部存在性路线仍未闭合；正文替换路线不证明该附录，也不证明光滑类与辅助分片类下确界相等。

Gilbarg–Trudinger、Vekua、Wall、Schoen 1983 按教材标准表述使用，未对照原书或章节。Schultens 核对的是 arXiv:0707.3926v4，未逐页核期刊版。FHS 文本系 OCR，公式可能识别错误。各项影响见 [open-items.md](proof/open-items.md)，来源状态见 [bibliography.md](sources/bibliography.md)。

本结论不认证全部 87 步独立通过、全论文、Theorems A/C/D、附录 C，或后续版本新增的存在性证明；没有人类专家认证。

## 目录导读

| 文件 | 内容 |
|---|---|
| [README.md](README.md) | 英文对应说明 |
| [proof/dependency-map.md](proof/dependency-map.md) | 七区段总图与 Mermaid 子图，区分黑箱输入和未闭合支路 |
| [proof/step-verification.md](proof/step-verification.md) | 全部 87 步的类型、比赛版定位、判定、理由及补法链接 |
| [proof/repairs.md](proof/repairs.md) | 全部英文补法与统一定量接口 |
| [proof/open-items.md](proof/open-items.md) | 未闭合路线、原书核对欠账及影响范围 |
| [sources/bibliography.md](sources/bibliography.md) | 文献版本、具体定理与页码、获取途径及 OCR 状态 |
| [LICENSE](LICENSE) | CC BY 4.0 适用范围与署名方式 |
| [MANIFEST.sha256](MANIFEST.sha256) | 除自身外各文件的 SHA-256 |

Mermaid 图可由 GitHub 原生渲染。在仓库根目录，macOS 可用 `shasum -a 256 -c MANIFEST.sha256` 检查文件完整性，GNU coreutils 可用 `sha256sum -c MANIFEST.sha256`。清单验证文件字节，不验证数学正确性。

## AI 说明

GPT-6.1 Sol performed the step decomposition, the line-by-line checks and an adversarial review, and drafted this package, in OpenAI Codex under human direction; Claude planned the process, checked key claims against the sources and reviewed the final text. No human expert has certified the work.

## 许可

本仓库原创文字在适用权利存在的范围内采用 **CC BY 4.0**。请署名 **apex-p01-seifert-exchange-lemma-verification contributors**，提供许可链接并注明修改；可取得时附仓库地址与使用版本。目标论文及第三方文献保留各自权利，不在本许可授予范围内。详见 [LICENSE](LICENSE)。
