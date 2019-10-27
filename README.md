# 大学物理题解编写临时仓库
本仓库存放大学物理题解的$\mathrm{\LaTeX}$代码、插图等

## 排版者任务

### 要求

- 自己敲代码，可以对原题解的解答格式进行修改，使尽量美观；利用软件将电子版文件转成.tex 文档时，对不整齐的代码进行**整理简化**；
- 格式和内容形式参照上学期的解析。不会用$\mathrm{\LaTeX}$的可以手写公式，或者mathtype都可以。但也需要考虑上学期那个的格式；
- 注意考虑到各种不同学习程度的同学的感受，**难题或理解深的题最好要深挖，要解释清楚，可给出多种解法；简单题的解答也要有完整的逻辑，不能“见课本”了事**。可以在解答之外写出自己的理解（参见上学期第四章开头）、其他相关练习等；
- ddl：每次作业下发后一周内完成，排版在编写完成后一周内完成。至于最后几章要紧张点，全部内容在期末考前两周完成，希望在考前出版，为同学所用（具体再调整）。
考虑到大家进度差不多，我就以自己班级的为准，到时候在群里问。

### 奖励
- 编写：每章12-16工时，不包括则扣除相应部分。根据内容、**质量**给工时。
- 排版：按内容贡献者所得工时的 60% 折算，向上取整。特殊情况另行商议。
- 审稿：一篇1-2工时，视资料长度而定。包括上学期的内容。能拉你的同学审稿也行啊。没分到任务的同学别退出啊！
- 增补他人题解内容/编写小专题/知识框架及理解/复习思维导图：视内容多少、质量而定。小专题参见《狭相小助手》。

## 组织者任务
- 每次收上来以后反馈不足之处给编写者，令其改正。
- 确定终稿。

## 尚未分配的任务
- 把上学期的.tex文件整理成分文件的形式
- 第十章的填空、解答题解析还未完成
- 勘误工作

## 排版整体要求和细节规范
详见[学研部排版学习路线](https://qyxf.site/technique/typeset)

### 配图

- 插图**必须美观**，可以拍已有印刷物的图、网上下或手绘较清晰的图，不美观就用电脑画。编写者能画尽量画好。
- 配图需要尽量使用矢量格式的图片，推荐使用 Tikz 包进行绘制。
- 亦可使用 `\includegraphics` 插入点阵图片 (.png .jpg 格式)
- 配图不要采用照片，如必须采用，可以经过处理软件处理为黑白图片后插入文档中
- 配图需注明图名，标上序号。序号按照章节、题目序号分配。如：「Chp12_21」

### 选择题、填空题

- 题目与题目之间（代码）空两行
- 选择题解析中尽量使用行内公式 `$ Your Equation Here $`
- 请尽量使用中文标点
- 表示流程使用`$\rightarrow$`，表示“可以推出”用`$\Rightarrow$`。
- 填空题中，多个空的答案使用`\qquad`命令分隔

### 解答题

- 题目与题目之间空一行
- 解答题解析中公式部分使用行间公式 `$$ Your Equation Here $$`或`gather`环境等
- 等号需对齐的多行公式使用`align`或`aligned`等环境
- 用$\because$和$\therefore$的解答方式，让解答过程左对齐，等号对齐
- 解答题解析中不要将文字部分放到公式环境中

### 模板中的命令

- 所有题目需使用 `\exercise` `\solve ` 命令
注：我把模板里的`\solve`改了，整体占两个字符，保证首行缩进一致。
- 导数、微分等使用`\di`等命令（见.tex模板）

### 分数

- 无论使用`\dfrac`还是`\frac`，需保证分数与上下的行不能靠太近
- 分数作为分子分母的分数，用斜杠作为分数线。如：${{{{\left(\frac{V_A/p_A}{V_B/p_B}\right)}^{\gamma-1}}}}$

### 某些字体的使用

- 单位最好用正体，用`\mathrm{}`
- 数学符号一定要斜体，放在数学环境中
- 化学式请使用`\ce{化学式(formula)}`，添加`\usepackage[version=4]{mhchem}`宏包
- 罗马数字使用如下命令：`\newcommand{\RNum}[1]{\uppercase\expandafter{\romannumeral #1\relax}}`
- 下标尽量不用汉字；如果一定要用的话，字号不能太大；可以附带文字说明其含义。

### 定界符、限制符
- 括号、绝对值符号建议加上定界符`\left`,`\right`

## 需要完善的题目

- 可能有些解析不够细致
- 12.6，解答没有任何文字说明
- 11,12章有两个插图需要重画。