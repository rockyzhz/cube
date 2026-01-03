# cube - 三阶魔方绘制 LaTeX 宏包

[![GitHub](https://img.shields.io/badge/GitHub-rockyzhz%2Fcube-blue.svg)](https://github.com/rockyzhz/cube)

`cube` 是一个用于绘制三阶魔方图形的 LaTeX 宏包，提供了简单的命令来表示魔方的各个面、块和颜色，支持 CFOP 公式的图形化展示。

## 功能特性

- **魔方三维绘制**：支持正二等轴测投影、正等轴测投影、斜投影等多种视角
- **颜色系统**：内置白色、黄色、蓝色、绿色、橙色、红色、黑色等颜色映射
- **公式可视化**：支持 FLL、OLL、PLL 等 CFOP 公式的图形化展示
- **箭头绘制**：提供魔方公式符号的箭头指示绘制功能
- **coffin 封装**：命令结果可直接用于 coffin 排版

## 快速开始

```latex
\documentclass{article}
\usepackage{ctex}
\usepackage{cube}

\begin{document}

% 绘制三面视图的魔方
\Cube{----b}{r--r-}{-----b---}
\Cube{---bb-bbb}{-r--rrrrr}{-----b---}
\Cube{rwryroobo}{bbwyyyywg}{gggbbwwow}
\Cube{bbbbbbbbb}{rrrrrrrrr}{yyyyyyyyy}

% 绘制魔方公式符号
\CubeNotation{U'}

\end{document}
```

## 示例效果

![CFOP 公式示例第1页](CFOP-preview-0.png)

![CFOP 公式示例第2页](CFOP-preview-1.png)

## 文件说明

| 文件 | 说明 |
|------|------|
| `cube.sty` | 宏包核心文件 |
| `cube.tex` | 宏包使用说明文档 |
| `CFOP.tex` | CFOP 魔方教程文档 |

## 依赖环境

- LaTeX2e
- TikZ (含 3d、calc、math、arrows.meta 库)
- xcoffins
- expl3 + l3regex-supplement
- xparse

## 作者

张泓知

## 许可证

MIT License
