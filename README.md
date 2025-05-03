# 住宅価格予測 - Kaggle Notebook プロジェクト

このプロジェクトは、Kaggle の「House Prices - Advanced Regression Techniques」コンペティションで提供されているデータセットを用いて、住宅価格を予測する機械学習モデルを構築したものです。

主に Kaggle 上で作成・実行した Notebook を GitHub にエクスポートし、ポートフォリオとして掲載しています。

---

## 📌 プロジェクトの目的

- Ames Housing データセットを用いた住宅価格の回帰予測
- モデル精度の最大化と過学習の抑制
- 機械学習ワークフロー（前処理・可視化・特徴量エンジニアリング・モデル構築・評価）の実践

---

## 📂 使用データ

- データソース：[Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- ファイル：
  - `train.csv`（学習用データ）
  - `test.csv`（予測対象データ）

---

## 🧪 使用ライブラリ

| ライブラリ名 | 用途 |
|--------------|------|
| pandas | データ処理 |
| numpy | 数値演算 |
| matplotlib / seaborn | データの可視化 |
| scikit-learn | 前処理、モデル評価、交差検証 |
| scipy | Box-Cox 変換などの統計処理 |
| lightgbm | モデル構築（勾配ブースティング） |

---

## 🔍 分析の流れ（Notebook 構成）

1. **データの読み込み**
2. **EDA（探索的データ分析）**
   - 相関分析、分布確認、欠損値チェック
3. **前処理・クリーニング**
   - 外れ値除去、欠損補完、カテゴリ変換
   - Box-Cox 変換による目的変数の正規化
4. **特徴量エンジニアリング**
5. **モデル構築**
   - LightGBM + 5-fold クロスバリデーション
   - 評価指標：RMSE
6. **予測結果の出力**
   - 提出ファイル `House_Prices.csv` を作成

---
