---  
title: Jekyllで外部リンクを新しいタブで開くように設定したい  
author: cachalot792  
date: 2024-01-23 13:50:00 +0900  
categories: [プログラミング]  
tags: [jekyll, githubpages, web, chirpy]  
---  

タイトルの通り、Jekyllで外部リンクを新しいタブで開くように設定するのが今回の目標です。  

## ポイント  

各記事はMarkdownで記述していますが、**mdファイル内にHTMLタグ等は書きたくありません。**  

Markdownの良さはそういうものを書かなくて済むところだと思っています。  

また、記事を書くたびにそうした記述が必要だと書き忘れてしまうリスクもあるので、一度の設定でサイト全体に適用される方法がベストです。  

## 方法  

今回、[Jekyll Target Blank](https://github.com/keithmifsud/jekyll-target-blank)というものを使用しました。  

まず、サイトのGemfileに以下のコードを追加します。  

```
gem 'jekyll-target-blank'
```

そして、_config.ymlに以下のコードを追加します。  

```
plugins:
  - jekyll-target-blank
```

たったこれだけです。超かんたん。  

## 所感  

「ね？簡単でしょ？」みたいな記事になってますが、自分が一番この簡単さに感動しました。  
