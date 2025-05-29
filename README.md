# 自動シフト作成システム

[![React](https://img.shields.io/badge/React-18.0+-blue.svg)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.0+-38B2AC.svg)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

従業員の条件や制約を考慮して、自動的に最適なシフト表を生成するWebアプリケーションです。

![シフト作成システムのスクリーンショット](./docs/screenshots/main-interface.png)

## 🌟 主な機能

### 📊 高度なシフト管理
- **自動シフト生成**: 複数の制約条件を考慮した最適化アルゴリズム
- **視覚的なシフト表**: 月別カレンダー形式での表示
- **リアルタイム統計**: 従業員別の勤務時間と負荷分析

### 👥 従業員管理
- **詳細プロフィール**: 雇用形態、スキルレベル、時給設定
- **勤務条件設定**: 最大勤務時間、連続勤務制限、希望シフト
- **個別制約管理**: NGシフト、実行不可業務の設定

### 🚫 制約・ルール管理
- **NG組み合わせ**: 従業員間の勤務制限設定
- **業務タスク管理**: カスタム業務の追加・編集・削除
- **必須ペア**: 一緒に勤務する必要がある従業員の設定
- **監督システム**: 監督者と監督が必要な従業員の管理

### ⚙️ 柔軟な設定
- **シフト別制約**: 各シフトの必要人員・業務要件
- **固定シフト**: 特定の日に固定で入るシフト
- **希望休設定**: カレンダー形式での休日希望入力

## 🚀 クイックスタート

### 前提条件
- Node.js 16.0以上
- npm または yarn

### インストール

```bash
# リポジトリをクローン
git clone https://github.com/yourusername/shift-scheduler.git
cd shift-scheduler

# 依存関係をインストール
npm install

# 開発サーバーを起動
npm start
```

アプリケーションは `http://localhost:3000` で起動します。

### ビルド

```bash
# 本番用ビルド
npm run build

# ビルドファイルをローカルで確認
npm run serve
```

## 📖 使用方法

### 1. 従業員の登録
1. 「従業員追加」ボタンをクリック
2. 基本情報（名前、雇用形態、時給など）を入力
3. 勤務条件（最大時間、勤務可能曜日など）を設定
4. 制約条件（NGシフト、実行不可業務など）を設定

### 2. 業務タスクの管理
1. 「業務管理」ボタンをクリック
2. 必要な業務タスクを追加・編集
3. 各従業員の実行不可業務を設定

### 3. NG組み合わせの設定
1. 「NG管理」ボタンをクリック
2. 一緒に勤務させたくない従業員の組み合わせを設定
3. NG理由も記録可能

### 4. シフト生成
1. 対象月を選択
2. 希望休をカレンダーで設定
3. 「シフト生成」ボタンをクリック
4. 自動的に最適なシフトが生成される

詳細な使用方法は [USAGE.md](./docs/USAGE.md) をご覧ください。

## 🛠️ 技術スタック

- **フロントエンド**: React 18+ with Hooks
- **スタイリング**: Tailwind CSS
- **アイコン**: Lucide React
- **状態管理**: React useState/useReducer
- **ビルドツール**: Create React App

## 📚 機能詳細

### シフト生成アルゴリズム
- 従業員の勤務可能日・時間制限を考慮
- NGコンビネーション・必須ペアの自動チェック
- 監督者配置の最適化
- 業務要件の自動満足
- 公平な勤務時間配分

### 制約チェック機能
- リアルタイム制約違反検出
- 詳細なエラーメッセージ表示
- 制約ルールの優先順位付け

機能の詳細については [FEATURES.md](./docs/FEATURES.md) をご覧ください。

## 🤝 コントリビューション

コントリビューションを歓迎します！以下の手順でお願いします：

1. このリポジトリをフォーク
2. 新しいブランチを作成 (`git checkout -b feature/amazing-feature`)
3. 変更をコミット (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュ (`git push origin feature/amazing-feature`)
5. プルリクエストを作成

## 📝 ライセンス

このプロジェクトは [MIT License](LICENSE) の下で公開されています。

## 🆔 作者

- GitHub: [@yourusername](https://github.com/yourusername)

## 🙏 謝辞

- [React](https://reactjs.org/) チーム
- [Tailwind CSS](https://tailwindcss.com/) チーム
- [Lucide](https://lucide.dev/) アイコンライブラリ

## 📞 サポート

バグ報告や機能要望は [Issues](https://github.com/yourusername/shift-scheduler/issues) でお願いします。

---

⭐️ このプロジェクトが役に立った場合は、ぜひスターを付けてください！
