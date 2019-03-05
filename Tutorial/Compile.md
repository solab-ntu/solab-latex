# Compile

## 普通文件

```bash
pdflatex file.tex
```

## 目錄 ```\tableofcontents```

pdflatex compiler does not support incremental compilation. It can't know how many chapters etc. are there in advance unless you would provide code right from the start that does a pre-definition (.toc).

```bash
pdflatex file.tex
pdflatex file.tex
```

## 引用文獻 ```\bibliography```

```bash
pdflatex file.tex
bibtex file.tex
pdflatex file.tex
pdflatex file.tex
```

