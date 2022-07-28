# 在 hard 模式 Reset 了某個 Commit，如何救回來?

> 先有一個觀念，無論什麼模式進行 Reset，Commit 並不會因為 Reset 就消失

- 使用 `reflog` 指令，查看 Commit Id

```bash
git reflog
```

- 使用 `--hard` 指令，強迫放棄 Reset 之後修改的檔案

```bash
git reset a5171ff --hard
```
