---
name: zhongguo-gudai-kongjian-xushi-lunwen-geshi
description: Use only for course-paper assignments by the 2024 cohort of the Chinese Language and Literature major at Shantou University that require the specific “中国古代小说空间叙事研究” format, including original-text quotation blocks, Chinese punctuation, footnotes, and references.
---

# 中国古代小说空间叙事论文格式

## 适用范围

本规范仅适用于汕头大学汉语言文学专业 2024 级的课程论文作业。其他年级、专业或用途的论文，请先确认其课程要求，不要默认套用本规范。

## Workflow

1. Preserve the user's content, existing valid footnotes, and document structure unless the user explicitly asks for text revision or deletion.
2. Work on a copy when editing an existing paper. Put the final copy where the user requested.
3. Use the `docx`/Word-processing workflow for `.docx` files. Inspect the actual OOXML when footnotes, styles, reference numbering, mixed Chinese/English font runs, or quotation marks matter.
4. Apply the formatting rules below consistently across the whole paper.
5. Verify after editing: open/read the produced `.docx`, count footnote references versus footnote bodies, and spot-check fonts,字号, bolding, alignment, indentation, line spacing, quotation marks, and reference order.

## Page And Body Formatting

- 大标题 / Main paper title: 黑体，四号，黑色，居中，不加粗.
- Abstract line: 宋体，小四. Only `摘要` is bold; the colon and abstract content are not bold.
- Keyword line: 宋体，小四. Only `关键词` is bold; the colon and keyword content are not bold.
- 章节标题 / Chapter-level headings such as `一、引言` or `二、……`: 宋体，小四，加粗，居中. Insert real blank paragraphs above and below; do not rely only on visual paragraph spacing.
- 带括号小标题 / Parenthesized section headings such as `（一）……` and `（二）……`: 宋体，小四，加粗，首行缩进两个中文字符. Insert real blank paragraphs above and below.
- Body text: 宋体，小四，固定行距 20 磅，首行缩进两个中文字符.
- 原著引文 / Original-text quotation blocks, especially quoted passages from classical works or《红楼梦》: 单独成段，仿宋，小四，固定行距 20 磅，上下空行.
- 中文双引号 / Chinese quotation marks must use Chinese curly quotes `“ ”`, never ASCII straight quotes ". Also ensure the quote-mark run itself uses 宋体; do not leave Chinese quotes inside a Times New Roman run.
- English words, English bibliographic material, and Arabic numerals may use Times New Roman where mixed-font formatting is required.
- Reference title: use `参考文献：`; format according to the chapter-title system unless a user-provided sample requires otherwise.

## Footnotes

- Preserve all valid existing footnotes. Remove footnotes only when the user explicitly identifies them as unwanted.
- Put the footnote marker after punctuation.
- Footnote numbering: circled-number style, restart numbering on each page.
- Footnote marker font: use Word theme font Calibri（正文）for both in-text footnote markers and footnote-area markers. In OOXML, prefer theme font attributes such as `asciiTheme="minorHAnsi"` and `hAnsiTheme="minorHAnsi"` instead of hard-coding `Calibri`.
- Ensure the `FootnoteReference` character style exists. It should include superscript behavior.
- Footnote body: 宋体，五号，固定行距 20 磅，段前 0，段后 0.
- Leave one visible space after the footnote marker before the footnote text, matching the course reference sample.
- If footnotes look like an extra blank line appears between entries, inspect and normalize all of these:
  - `Normal` style paragraph spacing: before `0`, after `0`.
  - `FootnoteText` style: do not let it introduce extra paragraph spacing.
  - Each actual footnote paragraph: spacing before `0`, after `0`, line `400`, `lineRule="exact"`.
  - Footnote separator and continuation separator paragraphs: compact spacing, e.g. after `0`, line `240`, auto.

## Citation Formats

- Monograph: author, title, place, publisher, publication date, volume/order if any, page number.
- Journal article: author, article title, place if required, journal title, issue/date, page number.
- Ancient text: author, article/work title, book title, juan number, and version information when available.
- For ancient authors, mark the dynasty before the author name at first full citation.
- English source: follow English academic citation conventions, e.g. `Leo Ou-fan Lee, The Romantic Generation of Modern Chinese Writers (Harvard University Press, 1973), p.208.`

## 《红楼梦》 Page Footnotes

When the user asks to add page footnotes for《红楼梦》quotations:

1. Use the specific edition/PDF/book named by the user as authoritative.
2. Match each quotation against that edition before assigning page numbers.
3. If the paper quote has minor textual variants, do not silently rewrite the quote unless the user asks; note or preserve the variant and still cite the corresponding page if the match is clear.
4. Add a《红楼梦》footnote to every actual quotation from the novel.
5. Do not cite non-novel material as《红楼梦》正文, such as literary criticism, historical edicts, or the user's own analysis.
6. First《红楼梦》footnote: include full bibliographic version information and page number. Use dynasty labels for ancient authors, for example: `[清]曹雪芹著；[清]无名氏续；中国艺术研究院红楼梦研究所校注：《红楼梦》，北京：人民文学出版社，2008年第3版，第38—39页。`
7. Later《红楼梦》footnotes: use a short form such as `《红楼梦》，第39页。`
8. For cross-page quotations, use the user's local convention, e.g. `第623—624页。`

## References

- Keep bracketed numbering such as `[1]`, `[2]`, `[3]`.
- Renumber references consecutively after sorting.
- Sort references in this order unless the user provides another sample:
  1. Chinese-language references before foreign-language references.
  2. Within Chinese references: books/monographs first, then journal articles, then dissertations, then web/network sources.
  3. Keep foreign-language references after Chinese references and preserve English punctuation/style.
- Chinese monograph: author, title `[M]`, place, publisher, publication date.
- Chinese journal article: author, article title `[J]`, journal title, issue/date.
- Dissertation: author, title `[D]`, school, year.
- Add the authoritative《红楼梦》edition used for page footnotes to the reference list and place it in the Chinese book/monograph group.

## OOXML/Word Implementation Notes

- Real blank lines: insert empty paragraphs above and below chapter headings and parenthesized section headings. Do not rely only on `before`/`after` spacing because course samples often expect visible blank paragraphs.
- Main title: remove `<w:b>` and `<w:bCs>`; keep 黑体, size `28` half-points, centered, color `000000`.
- 小四 is `w:sz="24"`; 五号 is `w:sz="21"`; fixed 20 pt line spacing is `w:spacing w:line="400" w:lineRule="exact"`.
- Footnote style definitions matter. If `FootnoteReference` or `FootnoteText` is missing in `word/styles.xml`, add or repair it; setting only run-level properties may still display incorrectly in Word.
- Calibri（正文）should be implemented as theme font attributes, not direct `Calibri`: use `asciiTheme="minorHAnsi"`, `hAnsiTheme="minorHAnsi"`, and suitable `cstheme`.
- Chinese quotes: replace straight quotes with `“ ”`, then split quote marks into their own runs and set those runs to 宋体. Character replacement alone is not enough if the run keeps Times New Roman.
- Footnote line-height problems often come from inherited style spacing or separator paragraphs, not from the footnote body text itself. Compare against a known-good reference document when possible.

## Verification Checklist

- Confirm the output `.docx` opens normally.
- Confirm footnote reference count equals footnote body count.
- Spot-check the main title: 黑体，四号，黑色，居中，不加粗.
- Spot-check chapter headings and parenthesized headings for 宋体，小四，加粗, correct alignment/indentation, and real blank paragraphs above and below.
- Spot-check body text for 宋体，小四，首行缩进两个中文字符，固定 20 磅.
- Spot-check original-text quotation blocks for 仿宋，小四，上下空行.
- Confirm there are no ASCII straight double quotes in visible text, and all Chinese quote-mark runs use 宋体.
- Spot-check footnote numbering: circled numbers, restart each page, marker font Calibri（正文）, footnote body 宋体五号 fixed 20 pt with no extra paragraph gap.
- Spot-check first and later《红楼梦》footnotes for full-form versus short-form citation, including dynasty labels in the first full citation.
- Confirm reference numbering is consecutive and sorted by the required order.
