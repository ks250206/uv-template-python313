# example-project

Python 3.13 を使用したプロジェクトテンプレート。uv、ruff、ty、pytest を使用した厳格な開発環境を提供します。

## 概要

このプロジェクトは以下のツールを使用しています：

- **uv**: 高速な Python パッケージマネージャー
- **ruff**: 高速な Python リンター・フォーマッター
- **ty**: 型チェッカー（mypy の代替）
- **pytest**: テストフレームワーク

## 要件

- Python 3.13
- uv

## セットアップ

```bash
# 依存関係のインストール
uv sync

# 開発環境のアクティベート
source .venv/bin/activate  # Linux/macOS
# または
.venv\Scripts\activate  # Windows
```

## 使用方法

```bash
# メインスクリプトの実行
uv run python src/main.py

# または
python src/main.py
```

## 開発

### リントとフォーマット

```bash
# リントチェック
uv run ruff check .

# 自動修正
uv run ruff check --fix .

# フォーマット
uv run ruff format .
```

### 型チェック

```bash
uv run ty
```

### テスト

```bash
# テストの実行
uv run pytest

# 詳細な出力
uv run pytest -v
```

## プロジェクト構造

```text
.
├── src/
│   ├── main.py          # メインスクリプト
│   └── main_test.py     # テストファイル
├── tests/               # テストディレクトリ
├── pyproject.toml       # プロジェクト設定
└── README.md           # このファイル
```

## ライセンス

LICENSE ファイルを参照してください。
