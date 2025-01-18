# GitHub Practice Repository

このリポジトリは、GitHubの基本操作を学習するための練習用リポジトリです。

## 目的
- GitHubの基本的な操作方法の習得
- Markdown記法の練習
- バージョン管理の基礎学習

## 学習内容
1. リポジトリの作成と基本設定
2. READMEの編集とMarkdown記法
3. コミットの作成と管理
4. ブランチの操作

## 備考
- Claude先生の指導のもと、学習を進めています
- このリポジトリは学習過程を記録するために公開しています

## ブランチの実験ゾーン
<details>
<summary>クリックして開く</summary>

ここに詳細な内容を書くことができます。
- リスト項目1
- リスト項目2

コードブロックも入れられます：
```python
print("Hello, GitHub!")
```
</details>

### 学習予定
- [x] リポジトリの作成
- [x] READMEの基本編集
- [ ] ブランチの操作理解
- [ ] マージの練習

### My GitHub Journey :rocket:
- :books: 学習中
- :bulb: アイデア
- :star: お気に入り

### 表
| 機能 | 説明 | 難易度 |
|-----|------|--------|
| コミット | 変更を記録 | ★ |
| ブランチ | 分岐を作成 | ★★ |
| マージ | 変更を統合 | ★★★ |

## Gitコマンドカンペ

### 投稿手順

#### 1. 変更状態の確認
```bash
git status
```
- 現在のブランチは？
```
git branch
```  

#### 2. ブランチの移動
- 移動する
```
git checkout 既存ブランチ名
```
```
git switch 既存ブランチ名
```
- 新規ブランチを作ってそっちへ移動
```
git switch -c 新規ブランチ名
```
```
git checkout -b 新規ブランチ名
```

#### 3. 新規・変更された投稿の追加
```bash
git add _posts/*.md
```

#### 4. 変更の確定（""内が変更内容のコメント）
- commit = ステージング（俎上に載せる）
```bash
git commit -m "Update posts"
```

#### 5. GitHubに反映：PR（Pull Request）
- マージを行うためのリモートへの「提案」
- 「このブランチの変更内容をmainに取り込んでいい？」という申請。
- この後にMergeが来る。
```bash
git push origin main
```

#### 6. ブランチの変更をmainにマージ（統合）：２つのブランチの内容を一つにまとめる
- mainブランチに移動してから、統合したいブランチ名を指定して`git merge`
```
git checkout main
git merge ブランチ名
```

#### 7. そのほか
- 現在のワークスペースで変更をすべて取り消し
```
git reset --hard origin/main
git clean -fd
```
- リポジトリの新規クローン
```
git clone https://github.com/toya-mimura/solpar.git workspace
cd workspace
```

