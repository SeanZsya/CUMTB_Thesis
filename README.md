# 中国矿业大学（北京） XeLaTeX 学位论文模板
CUMTB Thesis Template for Graduation Project (Undergraduate) 

依照[教务处最新（2021/1/19）规范](https://jwc.cumtb.edu.cn/info/1014/2205.htm)完成。

参考文献样式使用[国标GB/T 7714-2005](https://github.com/Haixing-Hu/GBT7714-2005-BibTeX-Style)。

目前仅提供本科毕业设计（论文）模板，请使用 XeTeX 引擎和 UTF-8 字符编码。

## 使用
### windows用户
#### 方法1：在TexLive环境下编译 

- 推荐使用`Visual Studio code`+`TeX Live`的组合

- 在`VS code`json配置文件中加入
```
"latex-workshop.latex.tools": [
    {
        "name": "xelatex",
        "command": "xelatex",
        "args": [
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "%DOC%"
        ]
    }
],
"latex-workshop.latex.recipes": [
    {
        "name": "xelatex -> bibtex -> xelatex*2",
        "tools": [
            "xelatex",
            "bibtex",
            "xelatex",
            "xelatex"
        ]
    }
]
```

- 编译顺序`xelatex` -> `bibtex` -> `xelatex` -> `xelatex`
#### 方法2：使用脚本文件
- 点击运行 build_thesis.cmd

- 如运行遇到问题，尝试以管理员身份打开

## Q&A
## Work Being Done
- [ ] 正文前页面的制作
- [ ] 编写模板类，接口留出，实现隐去
- [ ] 证明环境的编辑
- [ ] 转为 mian.tex-(part.tex)s 的总分模式
- [ ] 硕士、博士毕业论文制作
