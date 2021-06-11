Introduction for thesis
===

與之前 Template 採用的編譯器 pdflatex 不同， Thesis 是採用 xelatex 編譯，這邊需要多做一些設定。

Windows
---
1. 請確認 MikTex 更新為最新版
2. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
3. 請用 [SimpleXeCJK](./TestFile/simpleXeCJK/main.tex) 測試編譯環境是否設定成功

Ubuntu
---
1. 利用 Command Line 測試 `xelatex` 有安裝成功，註：終止 xeltax 請輸入指令 `x`
2. Ubuntu 一般並無內建 Times New Roman 或標楷體, 因此需額外安裝。
    - 複製 [Fonts](./Fonts) 資料夾內字型檔到 `/usr/local/share/fonts`
    - 執行 `sudo fc-cache -fv` 刷新字型清單
    - 到 LibreOffice Writer 確認有 Times New Roman 與 DFKai-SB(標楷體) 這兩個字型
3. 請用 [SimpleXeCJK](./TestFile/simpleXeCJK/main.tex) 測試編譯環境是否設定成功
