+++
title = 'コマンド ヒストリー'
date = 2025-02-06T16:00:00+09:00
draft = false
summary = 'あなたが最も利用しているコマンドは何でしょうか'
categories = ["Shell"]
tags = ["Shell", "乱文"]
+++

なんだか流行っていますね

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">ガチで計測するとこんな感じだった<br>1. vi (実はNeovimが起動する)<br>2. git<br>3. rg<br>4. cd<br>5. sudo<br>6. ls (クセで打ってるだけで実際はそんなに使ってない)<br><br>↓これで計測できる<br>history 0 | awk &#39;{print $2}&#39; | sort | uniq -c | sort -nr | head -n 10<a href="https://t.co/QYSd7ReZGt">https://t.co/QYSd7ReZGt</a></p>&mdash; yutkat (@yutkat) <a href="https://twitter.com/yutkat/status/1887318223957467201?ref_src=twsrc%5Etfw">February 6, 2025</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## Usage

### macOS (おおよそ zsh)

```zsh
history 0 | awk '{print $2}' | sort | uniq -c | sort -nr | head -n 10
```

### Linux (多分 Ubuntu おおよそ bash)

history の引数が消えただけです．

```bash
history | awk '{print $2}' | sort | uniq -c | sort -nr | head -n 10
```

## 2025年2月6日 22時27分

### Haruki (Client; macOS)

```txt
180 go
90 git
76 cd
67 python
52 ssh
41 ls
32 ping
29 nslookup
27 code
25 bun
```

### Sakuta (Server; Ubuntu)

```txt
207 cd
177 ls
94 docker
74 sudo
56 git
51 exit
40 nano
29 scp
21 ip
17 ssh
```

### Nodoka (Server; Ubuntu)

```
227 cd
171 ls
91 docker
78 sudo
58 kubectl
52 go
39 curl
33 nano
26 git
20 exit
```

### Kaede (Server; Ubuntu)

```
169 docker
142 cd
115 ls
44 sudo
21 curl
15 exit
10 rm
10 mkdir
8 code
8 cat
```
