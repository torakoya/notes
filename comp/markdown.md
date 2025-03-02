---
title: Markdown
created: 2025-03-02
---

なるべく汎用性のある書きかた（原典に定められていればもっともよい。あるいは GitHub Flavored Markdown に規定されているとか）で、簡潔に書け、見やすい書きかたをメモしておく。

Daring Fireball: Markdown \
<https://daringfireball.net/projects/markdown/>

GitHub Flavored Markdown Spec \
<https://github.github.com/gfm/>

CommonMark Spec \
<https://spec.commonmark.org/> \
GitHub Flavored Markdown が元にしたもの。こちらを見るほうがいいかも。

## 強制的な改行

原典では Markdown 文書に入れた改行は生成物では物理改行にならないと定めている。ただし Markdown パーサによってはそうするものもある。

強制的に改行するには、原典では行末にふたつ以上のスペースを入れることと定めている。しかしこれは気づきにくいから絶対に避けたい。

CommonMark では行末にバックスペースを入れる方法が用意されている。これがいいか。バックスペースの直前にスペースを入れたくなるが、入れると無視してくれないようだ（少なくとも GitHub と kramdown は。ただし入っていてもブラウザが無視してくれそう）。

## URL をリンクにする

Markdown 文書内の URL は、原典では自動的にリンクにはしてくれない。してくれるパーサもある。

URL をリンクにするもっとも簡潔な書きかたは、`<` と `>` でかこむこと。原典で定められている。
