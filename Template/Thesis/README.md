# Thesis

與之前的 Tutorial、Template 採用的編譯器 pdflatex 不同， Thesis 是採用 xelatex 編譯，這邊需要多做一些設定。

## Windows

1. 請確認 MikTex 更新為最新版
2. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
3. 請用 [SimpleXeCJK](./TestFile/simpleXeCJK/main.tex) 測試編譯環境是否設定成功

## Ubuntu

1. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
2. Ubuntu 一般並無內建 Times New Roman 或標楷體, 因此需額外安裝
    - 資料夾 [fonts](./fonts) 內有微軟的 Times New Roman 或標楷體
    - 請參考 Tutorial / Introduction 說明安裝字體
3. 可用 [test_files](./test_files/main.tex) 測試編譯環境是否設定成功
