+++
draft = false
date = 2022-06-02T21:01:33+09:00
title = "1.ターミナル無限ループ"
weight = 10
+++

アクテビティモニタで確認
→.zshrc(原因判明)
→source ~/.zshrc をファイルに書いてたので削除で解決

source ~/.zshrc source は現在の環境にファイルを読み込むということなので、
無限に読み込んでいたことがわかった。
<!--more-->