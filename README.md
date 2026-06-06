# Creator Type Diagnosis

クリエイタータイプ診断アプリです。

---

# 環境構築

## 必要環境

* Git
* Node.js
* npm

---

## Mac

### Node.js / npm インストール

Homebrew が入っている場合

```bash
brew install node
```

確認

```bash
node -v
npm -v
```

---

## Windows

### Node.js / npm インストール

以下から LTS版をインストール

https://nodejs.org/

確認

```bash
node -v
npm -v
```

---

# プロジェクトセットアップ

## 1. リポジトリをクローン

```bash
git clone <リポジトリURL>
cd creator-type-diagnosis
```

## 2. パッケージをインストール

```bash
npm install
```

## 3. 開発サーバー起動

```bash
npm run dev
```

表示されたURLへアクセス

例

```text
http://localhost:5173
```

---

# 開発フロー

## 最新コード取得

作業前に必ず最新状態へ更新

```bash
git switch main
git pull --rebase origin main
```

---

## 作業ブランチ作成

ブランチ命名規則

```text
自分の名前/実装内容
```

例

```bash
git switch -c ikehara/login
```

```bash
git switch -c ikehara/result-page
```

```bash
git switch -c toraga/header
```

---

## 作業内容をコミット

変更確認

```bash
git status
```

ステージング

```bash
git add .
```

コミット

```bash
git commit -m "ログイン画面を作成"
```

---

## GitHubへPush

初回Push

```bash
git push -u origin ブランチ名
```

例

```bash
git push -u origin ikehara/login
```

2回目以降

```bash
git push
```

---

## Pull Request作成

GitHub上で Pull Request を作成し、レビュー依頼を行ってください。

Pull Request タイトル例

```text
ログイン画面作成
```

---

# GitHub運用ルール

## Issue作成

作業前に Issue を作成する

例

```text
#1 ログイン画面作成
#2 診断結果画面作成
#3 ヘッダー作成
```

Issue と Pull Request を紐付ける場合

```text
close #1
```

を Pull Request の説明欄へ記載する。

マージ時に Issue が自動でクローズされる。

---

# 使用技術

* React
* Vite
* JavaScript
* Git
* GitHub

---

# ディレクトリ構成

```text
src/
├── components/
├── pages/
├── assets/
└── App.jsx
```

---

# 開発ルール

* main ブランチへ直接コミットしない
* main ブランチへ直接 Push しない
* 作業ごとにブランチを作成する
* Pull Request を作成してからマージする
* コミットメッセージは分かりやすく記載する
* 作業前に最新コードを取得する
* 作業前に Issue を作成する

---

# よく使うコマンド

最新コード取得

```bash
git pull --rebase origin main
```

ブランチ作成

```bash
git switch -c ikehara/login
```

コミット

```bash
git add .
git commit -m "ログイン画面作成"
```

Push

```bash
git push
```

現在のブランチ確認

```bash
git branch
```

変更確認

```bash
git status
```
