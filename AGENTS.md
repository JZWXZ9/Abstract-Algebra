# 抽象代数笔记项目约定

- 课程以群论为主；第一章课件是正文的主要依据，参考书为杨子胥《近世代数（第二版）》。新增课程课件后应优先按照实际课程调整。
- `ppt/` 和 `book/` 中原始资料只读。来源与页码见 `book/page_index.md`；PDF 阅读器页码和书本印刷页码不可混用。
- `notes/abstract-algebra.tex` 为主文件，`notes/chapters/chapterXX.tex` 为章节正文，`notes/elegantbook.cls` 是 ElegantBook 4.5 副本。`temp/chX/X.Y.md` 保存用户个人批注；未经用户要求，不改写或清除个人内容。
- 第 1 章已整理；第 2、3 章是以教材目录预置的框架，不代表已确认课程覆盖范围。环、域暂不纳入。
- 正文采用中文及 ElegantBook fancy 环境，例如 `\begin{definition}{名称}{标签}`、`\begin{theorem}{名称}{标签}`、`proof`、`example`、`remark`。有编号定理环境的标签由模板自动添加 `def:`、`thm:` 等前缀。
- 每节自动整理内容仅置于 `% >>> AUTO-GENERATED: X.Y — DO NOT EDIT MANUALLY <<<` 与 `% <<< END AUTO-GENERATED: X.Y <<<` 之间。后续整理时保留标记之外的正文与用户批注；不得覆盖 Markdown 中用户内容。
- 参考 PDF 的 OCR 仅用于检索；涉及公式、量词和证明时查看原始页面核验，无法看清就明确标注，不得凭 OCR 猜测。索引中记录来源文件、PDF 页及可确认的印刷页。
- 从 `notes/` 目录运行 `xelatex -interaction=nonstopmode -halt-on-error abstract-algebra.tex` 两次；检查编译日志和生成的 PDF 布局。
