# Citation

參考資料 [Overleaf / Bibtex\_bibliography\_styles][1]

[1]: https://www.overleaf.com/learn/latex/Bibtex_bibliography_styles

## 命令

```latex
\bibliographystyle{stylename}
\bibliography{bibfile}
```

## 樣式 stylename

影響文中引用文獻的編號、排序、格式，預設支援的樣式共有八種，其中我們常用的是 ieeetr。

- plain
- unsrt
- alpha
- abbrv
- acm
- apalike
- ieeetr
- siam

## 文獻管理

在開始寫論文後，會發現加 citation 是一件很費時的事情，這邊建議使用一些軟體來幫忙管理文獻。我目前是使用 Mendeley (https://www.mendeley.com/)。把文獻 pdf 檔加入後，這個軟體會自動幫忙搜尋或偵測該 pdf 的 citation，且可以輸出成 bibtex 的格式，因此只要在軟體中確認文獻資訊沒錯，就可以直接輸出使用。

在 Tools->Options->BibTex 中 Enable BibTeX syncing 就可以在每次 sync 時更新一個 library.bib 檔案在指定的資料夾，相當方便。只要將設定 `\bibliography{IEEEabrv,library}` 為同樣的檔名就可以在論文中歡樂的 cite 了。

另外要小心，在文件管理員中雙擊副檔名為 .bib 的檔案時，若預設由 mendeley 開啟，開啟的瞬間 mendeley 就會開始瘋狂匯入檔案，若你只是想點開來看看學長姐的.bib檔就會很尷尬。
