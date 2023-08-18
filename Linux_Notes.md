# Linux Command Line Notes

+ [ls 列出資料夾](#ls-列出資料夾)
+ [rm 刪除](#rm-刪除)
+ [grep 印出符合條件](#grep-印出符合條件)
+ [head、tail 觀看檔案頭尾](#headtail-觀看檔案頭尾)
+ [watch 重複執行固定指令](#watch-重複執行固定指令)
+ [chmod 控制對文件權限](#chmod-控制對文件權限)
+ [nslookup 查詢DNS](#nslookup-查詢dns)
+ [find 查詢檔案](#find-查詢檔案)
+ [vim shortcut](#vim-shortcut)
+ [history 歷史命令](#history-歷史命令)
+ [Ctrl + R 歷史命令搜尋](#ctrl--r-歷史命令搜尋)
+ [netstat 查詢網路資訊](#netstat-查詢網路資訊)
+ [awk 格式辨認與語言處理](#awk-格式辨認與語言處理)

### ls 列出資料夾

> -a -> 所有 \
> -l -> 條列式 \
> -t -> 異動時間 \
> -r -> 反向

```bash
ls -ltr
```

### rm 刪除

> -d -> 資料夾 \
> -f -> 強制 \
> -r -> 循環

```bash
rm -rf $dir
```

### grep 印出符合條件
> -c -> 數量
> -i -> 不分大小寫
> -n -> 列出行數
> -v -> 反向

```bash
grep $pattern $file -c
grep $pattern $file -ivn
```

### head、tail 觀看檔案頭尾

> -n $line -> 數目\
> -f -> 持續(只能用在tail)

```bash
tail -f $file
```

### watch 重複執行固定指令

> -n $second -> 間隔時間

```bash
watch -n 1 cat $file
```

### chmod 控制對文件權限

> role+$action \
> u -> user \
> g -> group \
> o -> other

```bash
chmod ugo+x $file
```

### nslookup 查詢DNS

```bash
nslookup google.com
```

### find 查詢檔案

```bash
find $file
```

### vim shortcut

> search
```bash
/$target
```

> paste
```
Shift + Insert
```

> find and replace in current line
```bash
:s/$target/$substitute/g
```

> find and replace all
```bash
:%s/$target/$substitute/g
```

> find and replace each with asking
```bash
:%s/$target/$substitute/gc
```

> find whole words and replace
```bash
:%s/\<$target\>/$substitute/gc
```

> next occur
```bash
n
```

> previous occur
```bash
N
```

> beginning of context
```bash
gg
```

> end of context
```bash
G
```
> delete line
```bash
dd
```

> delete all content
```bash
:%d
```

### history 歷史命令

### Ctrl + R 歷史命令搜尋

### netstat 查詢網路資訊

> -a -> 全部 \
> -t -> tcp \
> -u -> udp \
> -l -> 正在監聽 \
> -p -> 被哪個應用程式使用 \
> -n -> 不解析DNS

### awk 格式辨認與語言處理
