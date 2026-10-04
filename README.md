<div align="center">

# 🎓 华南理工大学（SCUT）研究生开题报告与文献综述 LaTeX 模板

### South China University of Technology · Graduate Research Proposal & Literature Review · 2026

**⭐ 如果这个模板帮你省下了排版时间，欢迎点击右上角 Star 支持一下！**

让更多有需要的同学找到它，也方便自己下次回来使用。

[![GitHub Stars](https://img.shields.io/github/stars/Wukong-SCUT/-Latex-?style=for-the-badge&logo=github&label=Star%20%E6%94%AF%E6%8C%81&color=E3B341)](https://github.com/Wukong-SCUT/-Latex-/stargazers)
![Version](https://img.shields.io/badge/版本-2026-9B2335?style=for-the-badge)
![Compiler](https://img.shields.io/badge/编译器-XeLaTeX-008080?style=for-the-badge&logo=latex)
[![Overleaf](https://img.shields.io/badge/在线编辑-Overleaf-47A141?style=for-the-badge&logo=overleaf)](https://www.overleaf.com/)
[![TeXPage](https://img.shields.io/badge/在线编辑-TeXPage-2563EB?style=for-the-badge)](https://www.texpage.com/)

**[📥 下载开题报告](https://github.com/Wukong-SCUT/-Latex-/raw/refs/heads/main/%E5%BC%80%E9%A2%98%E6%8A%A5%E5%91%8A.zip)** · **[📥 下载文献综述](https://github.com/Wukong-SCUT/-Latex-/raw/refs/heads/main/%E5%BC%80%E9%A2%98%E7%BB%BC%E8%BF%B0.zip)**

</div>

---

> [!IMPORTANT]
> **这是个人整理分享的 2026 版 LaTeX 模板，并非学校或学院官方发布的 LaTeX 模板。**
> 使用前请核对研究生院、所在学院及导师的最新要求；本仓库不保证模板符合每个学院、专业或具体提交环节的文件要求。

## 📦 模板下载

本仓库分享华南理工大学（South China University of Technology，SCUT）研究生学位论文开题报告与文献综述的 2026 版 LaTeX 模板，支持 XeLaTeX 编译，可在 Overleaf 或 TeXPage 中使用，方便在现有框架上填写个人信息、撰写正文和调整格式。

| 模板 | 下载文件 | 主文件 | 主要填写位置 |
| :--- | :--- | :--- | :--- |
| 研究生学位（毕业）论文开题报告 | [开题报告.zip](https://github.com/Wukong-SCUT/-Latex-/raw/refs/heads/main/%E5%BC%80%E9%A2%98%E6%8A%A5%E5%91%8A.zip) | `main.tex` | `metadata.tex`、`sections/` |
| 研究生学位（毕业）论文文献综述 | [开题综述.zip](https://github.com/Wukong-SCUT/-Latex-/raw/refs/heads/main/%E5%BC%80%E9%A2%98%E7%BB%BC%E8%BF%B0.zip) | `main.tex` | `main.tex` 中的填写区与正文 |

两个 ZIP 分别是独立工程，内含 LaTeX 源文件、封面图片和各自的使用说明。**请下载所需的单个模板 ZIP，并分别建立项目。** GitHub 的 `Code → Download ZIP` 下载的是整个仓库，使用在线平台时请先解压，再上传里面的模板 ZIP。

**快速导航：** [在线使用](#-在线使用推荐) · [本地编译](#-本地编译) · [填写位置](#-填写与修改) · [常见问题](#-常见问题) · [版本与责任说明](#-版本与责任说明)

## 🚀 在线使用（推荐）

推荐使用 **[Overleaf](https://www.overleaf.com/)** 或 **[TeXPage](https://www.texpage.com/)**，在浏览器中编辑、编译和预览 PDF，省去本地配置 LaTeX 环境的步骤。

### Overleaf

1. 下载上方的 `开题报告.zip` 或 `开题综述.zip`。
2. 登录 Overleaf，在项目列表中选择 **New project**，使用上传 ZIP 项目的选项（界面可能显示为 **Existing project (.zip)** 或 **Upload Project**），上传所需模板。
3. 打开项目设置，将 **Compiler（编译器）设为 `XeLaTeX`**，确认 **Main document（主文件）为 `main.tex`**。
4. 填写个人信息、替换正文和占位内容，点击 **Recompile** 编译。
5. 检查 PDF 的分页、字体、表格与签名区，确认符合提交要求后下载 PDF。

可参考官方说明：[上传 ZIP 工程](https://docs.overleaf.com/managing-projects-and-files/uploading-a-project) · [选择编译器](https://docs.overleaf.com/getting-started/recompiling-your-project/selecting-a-tex-live-version-and-latex-compiler)。

### TeXPage

1. 下载所需模板 ZIP，登录 TeXPage，通过**上传项目**导入该 ZIP。
2. 打开项目顶部的**设置**，确认主文件为 **`main.tex`**，编译器为 **`XeLaTeX`**。
3. 修改个人信息和正文，点击**编译**，检查预览结果并下载 PDF。

界面操作可参考 [TeXPage 官方使用教程](https://latex-static.texpage.com/9a3e551d-8f48-468e-acad-c5ee3fe59044)。

> [!TIP]
> **两个模板都使用 XeLaTeX。** 遇到 `fontspec` 或中文字体相关报错时，先检查编译器设置。上传时请保留完整工程，包含 `assets/`、`sections/` 等文件夹；只上传 `main.tex` 会缺少图片或被引用的文件。

## 💻 本地编译

安装带有中文支持的 TeX Live 或 MiKTeX，解压所需模板，在其 `main.tex` 所在目录运行：

```bash
xelatex main.tex
xelatex main.tex
```

通常连续编译两次，可更新交叉引用和页码。也可以使用已安装的 `latexmk` 自动完成必要的编译轮次：

```bash
latexmk -xelatex main.tex
```

如果使用 TeXstudio 或其他编辑器，请将编译器配置为 **XeLaTeX**，并以 `main.tex` 为主文件。

## ✍️ 填写与修改

### 开题报告

在 `metadata.tex` 中集中修改姓名、导师、学号、院系、专业、中英文题目、关键词和封面日期；对应信息会用于封面及相关表格。

正文按文件拆分，便于分块填写：

| 文件 | 内容 |
| :--- | :--- |
| `sections/01-abstract.tex` | 摘要 |
| `sections/02-basis.tex` | 立题依据 |
| `sections/03-research-plan.tex` | 研究方案 |
| `sections/04-foundation.tex` | 研究条件与基础 |
| `sections/05-schedule.tex` | 工作进度安排 |
| `sections/06-expected-results.tex` | 预期成果 |
| `sections/07-review-comments.tex` | 开题审核意见 |
| `sections/08-department-comments.tex` | 院（系）意见 |

审核、签名与审批栏请按实际流程填写。表格尺寸、签名区等排版细节在 `main.tex` 中调整，字体配置在 `fontsetup.tex` 中。

博士／硕士及相关选框默认为空，可在对应定义中将 `\square` 改为 `\boxtimes`。末尾默认附有定密审批表；是否需要保留，请依据实际要求决定。如需隐藏，在 `metadata.tex` 中将 `\showconfidentialformtrue` 改为 `\showconfidentialformfalse`。

### 文献综述

在 `main.tex` 的“填写区”修改个人信息、封面日期、综述题目与作者姓名，再将摘要、关键词、章节正文和参考文献示例替换为自己的内容。

- 将 `\showhintstrue` 改为 `\showhintsfalse`，可隐藏蓝色提示。
- 将 `\showinstructionstrue` 改为 `\showinstructionsfalse`，可隐藏说明页；是否保留请按提交要求决定。
- 黑色写作提示、`×××` 等占位文字及重复的参考文献示例仍需自行替换或删除。
- `references.bib` 初始为空；自动生成参考文献列表还需要配置文献条目、引用命令及参考文献样式，不能只向该文件添加条目就视为完成。

两个模板都预留了个人信息和写作内容，**请根据真实研究工作自行撰写**。压缩包内的 `README.md` 提供了更具体的填写与排版说明。

## 🔎 常见问题

**为什么中文字体与 Word 模板看起来略有不同？**  
模板优先读取相应的本机字体或 `fonts/` 中的字体文件，缺少时回退到 TeX Live 自带的 Fandol 字体。不同字体可能改变字形、换行和分页。如果学院明确要求宋体、黑体或仿宋，请按压缩包内说明配置自己有权使用的对应字体；模板不附带 Windows 商业字体文件。

**为什么填写后页数变多、表格挤出页面？**  
正文长度和字体会影响排版，部分签名与行政表格不适合自动跨页。请检查内容长度、表格高度和留白，必要时调整，尤其要在最终导出的 PDF 中核对分页与签名区。

**能否直接编译后就上交？**  
请先完成个人信息、日期、学位类别、正文和参考文献，清理占位内容，并逐项核对学院要求。编译成功仅说明生成了 PDF，不能代替提交格式检查。

## 📌 版本与责任说明

**本仓库分享的是 2026 版模板。** 开题报告工程根据《研究生学位（毕业）论文开题报告2026.4.13.docx》整理，文献综述工程根据相应的 Word 模板整理。年份用于标识本次分享版本，不表示模板已获得学校或所有学院的认可，也不表示后续要求不会变化。

- **分享范围：** 本仓库仅提供 LaTeX 模板与使用说明，供学习、排版和写作参考，不代写研究内容，不提供提交审核或格式认证。
- **要求优先：** 学校、研究生院、学院、专业及导师的要求可能不同，也可能更新。具体内容、格式、参考文献规范、签字盖章、提交文件类型及流程，以使用者收到的最新正式要求为准；要求使用指定 Word 表格或其他格式时，请按要求提交。
- **适用性：** 本仓库不保证模板满足每个学院或每次提交的要求，也不保证 LaTeX 输出与原 Word 模板逐页、逐行一致。模板内保留的填写提示与格式示例，请结合最新要求核对。
- **使用责任：** 使用者应自行检查最终文件的内容、版式与完整性，并完成必要修改。模板作者不对使用本模板产生的格式不符、退回修改或提交结果作出保证。

## 🤝 反馈与分享

欢迎通过 [Issues](https://github.com/Wukong-SCUT/-Latex-/issues) 反馈编译或排版问题。描述时请附上使用的平台、编译器、报错信息或相关页面截图，并注明模板类型；涉及具体学院要求时，请说明要求来源，方便判断适用范围。

欢迎把仓库分享给有需要的同学，也欢迎在分享时保留仓库链接。

---

<div align="center">

**祝开题顺利，写作顺利！**

如果用得顺手，别忘了点亮右上角的 **⭐ Star**。

</div>
