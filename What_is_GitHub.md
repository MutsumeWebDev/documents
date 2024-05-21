
# このドキュメントの目的

- リポジトリをクローンしてブランチして機能追加してコミットする、の意味を理解する/できるようにする
- GitHubを用いて、バージョン管理を適切に行いながら開発が行えるようにする

# 概論

Google Driveにファイルを追加して書き換えて、それをもとにまた書き換えて...  
これのデメリットはたくさんある。挙げてみよう

- 間違えて以前のデータを消しちゃったけど戻せない！
- 誰かがDriveの中身を変えたら毎回それを手動でダウンロードしないといけない
- 変更された場所が分かりづらい
- 同時並行で機能追加・開発がしづらい

上記のようにデメリットが多い。これを解決したいという動機がわく  
そのようなときに便利なのがGitによるバージョン管理とGitHubによるクラウド管理（のようなモノ）である

## 前提知識

### GitとGitHub

#### Gitとは？

ファイル群をバージョン管理するためのツール  
各PCにそれぞれ入っていて、「誰が」「いつ」「どこを」変更したのかという履歴を保存する  
また、その履歴から、復元したり差分を確認したりすることができる  

#### GitHubとは？

Gitをクラウド的に使えるようにするためのサービス  
Web上にファイル群を保存し、各PCからGitを通して変更履歴の送受信をする  
グループで開発をしやすくするための機能がいくつか追加されている  

#### 違いを見る

![Git and GitHub](images/git.png)

### 用語

> [!NOTE]
> [サル先生のGit入門](https://backlog.com/ja/git-tutorial/)

#### 一般編

- リポジトリ (Repository)
  - バージョン管理をされるファイル群（フォルダ）の情報が詰まったデータベースのようなもの

> [!IMPORTANT]
> リポジトリは、作業フォルダ（やその中のファイル類）と異なる  
> バックアップやセーブデータのように、別に保存されていると考えたほうが分かりやすい

- ローカルリポジトリ (Local Repository)
  - 各PCごとに作成されるリポジトリ、Gitで管理する
- リモートリポジトリ (Remote Repository)
  - ネットワーク上で管理されるリポジトリ、今回はGitHub上にある

> [!NOTE]
> [この記事の図](https://qiita.com/Coa3/items/d0a43b22a130f74a2685#2-git%E3%82%92%E7%90%86%E8%A7%A3%E3%81%99%E3%82%8B)を見るとわかりやすいかも

- コミット (Commit)
  - 作業フォルダの内容を、ローカルリポジトリ（特定のブランチ）に記録すること
- メインブランチ (Main Branch)
  - リポジトリの主となるブランチ
  - 基本的に異常がない状態にされる
- ブランチ (Branch)
  - あるブランチから分岐させて
- マージ (Marge)
  - あるブランチを他のブランチ（例えばMainブランチ）に取り込むこと

#### Git-GitHub間編

- クローン (Clone)
  - リモートリポジトリ（の特定のブランチ）の内容をコピーし、ローカルリポジトリにコピーすること
- プル (Pull)
  - リモートリポジトリの変更内容をローカルリポジトリに反映させること
- プッシュ (Push)
  - ローカルリポジトリの変更内容をリモートリポジトリに反映させること

---

# GitHubを使おう

## 実際の開発の流れ

### GitHub上での操作

### VSCode上でGitHubのコマンドを使う

## GitHub CLI コマンド集

> ref.
>
> [GitHubを完全に理解したい #1 Gitを理解する](https://qiita.com/Coa3/items/d0a43b22a130f74a2685)  
> [君には1時間でGitについて知ってもらう(with VSCode)](https://qiita.com/jesus_isao/items/63557eba36819faa4ad9)  
> [Gitの仕組みと用語 / GitHub Term](https://speakerdeck.com/kaityo256/github-term)  