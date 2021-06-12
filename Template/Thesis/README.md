# Thesis

## 前言

臺灣大學碩博士論文 XeLaTeX 模版

這個模版的前身是 LaTeX+CJK 的模版，如果您還是想用 LaTeX+CJK，請參考 [這篇文章](http://www.csie.ntu.edu.tw/~tzhuan/www/resources/ntu/)。

您可以直接 clone 這個 git repository，或者您可以在 [這裡](https://github.com/tzhuan/ntu-thesis/tags) 下載發行版本。

請參考 [wiki](https://github.com/tzhuan/ntu-thesis/wiki) 的說明。

## 注意

### Windows

1. 請確認 MikTex 更新為最新版
2. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
3. 請用 [SimpleXeCJK](./TestFile/simpleXeCJK/main.tex) 測試編譯環境是否設定成功

### Ubuntu

1. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
2. Ubuntu 一般並無內建 Times New Roman 或標楷體, 因此需額外安裝
    - 資料夾 [fonts](./fonts) 內有微軟的 Times New Roman 或標楷體
    - 請參考 Tutorial / Introduction 說明安裝字體
3. 可用 [test_files](./test_files/main.tex) 測試編譯環境是否設定成功
