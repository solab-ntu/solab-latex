# Compile

## TeXworks

工具列 File -> Preference 可以看到下圖視窗，可以看到編譯程式與順序。

![](./pics/Compile-texworks-setup.png)

點擊主程式下圖按鈕可以開始編譯文件。

![](./pics/Compile-texworks-start.png)

## VSCode

按下 Ctrl+Shift+P 執行命令，執行 LaTeX Workshop: Build LaTeX project。

![](./pics/Compile-vscode1.png)

其編譯程序可以打開 settings.json 設定，如下圖 latex-workshop.latex.tools 與 latex-workshop.latex.recipes 兩個變數，其內容可以參考下一節 Terminal 命令。

![](./pics/Compile-vscode2.png)

## Terminal

直接在 terminal 輸入命令進行編譯。

latex 編譯器不支援增量編譯，因此當文件中有目錄時，則需要 .toc 檔存在才能將目錄加入文件，同理，當有引用文獻時，則需要 .aux 檔存在。因此根據文件內容的不同，時常會使用好幾次命令執行編譯。

- 文件
```bash
pdflatex file.tex
```

- 目錄 \tableofcontents
```bash
pdflatex file.tex
pdflatex file.tex
```

- 文獻 \bibliography
```bash
pdflatex file.tex
bibtex   file.aux
pdflatex file.tex
```

