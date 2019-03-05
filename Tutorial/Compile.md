# Compile

## TeXworks

工具列 File -> Preference 可以看到下圖視窗，可以看到編譯程式與順序。

![](./pics/Compile-texworks-setup.png)

點擊主程式下圖按鈕可以開始編譯文件。

![](./pics/Compile-texworks-start.png)

## VSCode

按下 Ctrl+Shift+P 執行命令，執行 LaTeX Workshop: Build LaTeX project。

![](./pics/Compile-vscode1.png)

其編譯程序可以打開 settings.json 設定，如下圖 latex-workshop.latex.tools 與 latex-workshop.latex.recipes 兩個變數。

![](./pics/Compile-vscode2.png)

## Terminal

直接在 terminal 輸入命令。

### 文件

```bash
pdflatex file.tex
```

### 目錄 ```\tableofcontents```

pdflatex compiler does not support incremental compilation. It can't know how many chapters etc. are there in advance unless you would provide code right from the start that does a pre-definition (.toc).

```bash
pdflatex file.tex
pdflatex file.tex
```

### 引用文獻 ```\bibliography```

```bash
pdflatex file.tex
bibtex   file.aux
pdflatex file.tex
pdflatex file.tex
```

