# git_simple_commit_message_editor

## What is this?

這是一個對話式 commit 編寫工具
可以幫助團隊盡量寫出相同形式的 commit message

![](https://raw.githubusercontent.com/shimokei53/git_simple_commit_message_editor/master/tty.gif)

## How to use

```
$ chmod +x gscme
$ mv gscme /usr/local/bin/gscme

# 以下為 optional, 也可以直接使用 gscme 指令來使用這個 script
$ git config --local core.editor gscme
```

merge 或 rebase 的時候會直接啟動編輯器。
可以在 `CORE_EDITOR` 中設定您喜歡的 Editor。

## 會詢問的問題
會以一行一行的對話形式呈現。
內容可以在專案資料夾中的 `.gscme_msglist` 設定。
這個檔案可以在開發團隊中共享，讓 commit message 形式盡量統一。
