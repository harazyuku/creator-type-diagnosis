# Creator Type Diagnosis

クリエイタータイプ診断アプリです。

## 環境構築

### 1. リポジトリをクローン

```bash
git clone <リポジトリURL>
cd creator-type-diagnosis
```

### 2. パッケージをインストール

```bash
npm install
```

### 3. 開発サーバーを起動

```bash
npm run dev
```

ブラウザで表示されたURL（通常は http://localhost:5173 ）にアクセスしてください。

---

## 開発フロー

### ブランチ作成

main ブランチから作業用ブランチを作成します。

```bash
git switch main
git pull origin main
git switch -c feature/機能名
```

例:

```bash
git switch -c feature/top-page
```

### 作業内容をコミット

```bash
git add .
git commit -m "トップページを作成"
```

### GitHubへプッシュ

```bash
git push origin feature/機能名
```

### Pull Request作成

GitHub上で Pull Request を作成し、レビュー依頼を行ってください。

---

## 使用技術

* React
* Vite
* JavaScript
* Git / GitHub

---

## ディレクトリ構成

```text
src/
├── components/
├── pages/
├── assets/
└── App.jsx
```

---

## 開発ルール

* main ブランチへ直接コミットしない
* 作業ごとにブランチを作成する
* 作業完了後は Pull Request を作成する
* コミットメッセージは分かりやすく書く

## ブランチは　自分の名前/実装した内容　で記載

main
├─ ikehara/login
├─ ikehara/result-page
├─ friend/header
└─ friend/question-data
