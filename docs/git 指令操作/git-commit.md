# git 指令操作

## restore hard reset commit

無論什麼模式下進行 Reset，Commit 並不會使用 Reset 就消失

```bash
git reflog
```

- 使用 `reflog` 指令，可查看操作記錄

```bash
git reset a5171ff --hard
```

- 使用 `--hard` 指令，強迫放棄 Reset 之後修改的檔案
