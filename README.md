EN

Goal:

Early screening of depression risk (PHQ-9 ≥ 10) using behavioral social media signals.
This project builds a reproducible ML pipeline focused on:
Leakage-safe data splitting
LightGBM modeling with Optuna hyperparameter optimization
PR-AUC–oriented evaluation (class imbalance aware)
Validation-based threshold selection
Reproducible inference artifact (pipeline + threshold)

Final Model (v1.0):

Model: LightGBM (sklearn API)
CV objective: PR-AUC (5-fold)
Test PR-AUC: ~0.60 (baseline prevalence ~0.21)
Test Recall: ~0.83
Test Precision: ~0.51
Threshold selected on validation only
The model prioritizes risk detection (screening scenario) while maintaining moderate precision.

JP

目的:

ソーシャルメディア利用行動から PHQ-9 ≥ 10 を予測し、
うつ症状リスクの早期スクリーニングを行う。
本プロジェクトでは以下を重視した再現可能なMLパイプラインを構築した：
リーク対策済みデータ分割
Optuna による LightGBM 最適化
不均衡を考慮した PR-AUC 評価
Validation による閾値選択
推論用成果物（パイプライン＋閾値）の保存

最終モデル（v1.0）:

モデル: LightGBM（sklearn API）
CV目的関数: PR-AUC（5-fold）
Test PR-AUC: 約0.60（ベースライン約0.21）
Tet Recall: 約0.83
Test Precision: 約0.51
閾値は validation で選択
本モデルはスクリーニング用途として
リスク検出を優先する設定になっている。
