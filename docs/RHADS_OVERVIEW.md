# RHADS 製品概要

## RHADS とは

**Red Hat Advanced Developer Suite（RHADS）** は、開発者のセルフサービスとソフトウェアサプライチェーンの信頼強化をまとめたプレミアムな製品スイートです。  
開発者ポータルを起点に、成果物の署名・SBOM / リスク可視化などを一貫して扱えるようにします。

以前は Trusted Application Pipeline として語られていた流れがあり、現在は RHADS 配下のオファリングとして整理されています。

## 中核コンポーネント

| 略称 | 製品名 | 一言で |
|------|--------|--------|
| **RHDH** | Red Hat Developer Hub | Backstage ベースの社内開発者ポータル。カタログ、テンプレート、Docs、プラグイン |
| **RHTAS** | Red Hat Trusted Artifact Signer | Sigstore 系。成果物・メタデータなどの署名と検証、監査可能な証跡 |
| **RHTPA** | Red Hat Trusted Profile Analyzer | SBOM 管理、依存関係リスク、脆弱性・ライセンスなどの可視化 |

### 役割分担（覚え方）

```text
RHDH  … 「入口・黄金経路・セルフサービス」
RHTAS … 「本物か・改ざんされていないか（署名）」
RHTPA … 「中身は何か・どんなリスクか（SBOM / 分析）」
```

## Software Supply Chain（SSC）文脈で一緒に出るもの

RHADS - SSC の説明では、次もパイプライン全体の一部として言及されることが多いです。

| 製品 / 機能 | 役割 |
|-------------|------|
| **RHACS**（Advanced Cluster Security） | コンテナ／クラスタ観点の脆弱性・ポリシー |
| **OpenShift Pipelines**（Tekton 等） | CI（ビルド・テスト・デプロイの自動化） |
| **OpenShift GitOps** | CD / GitOps（宣言的な配信と環境同期） |

これらは「ポータルと信頼レイヤ」を、実際のビルド〜デプロイの流れにつなぐ部品です。ハンズオンでは環境により触れる範囲が異なります。

## 典型的な価値ストーリー（短く）

1. 開発者は **RHDH** のテンプレートから標準化されたプロジェクトを起こす  
2. パイプラインでビルドし、必要に応じて **署名（RHTAS）** と **SBOM / 分析（RHTPA）** が入る  
3. ポリシーやスキャン（**RHACS** 等）を経て、GitOps などで環境へ届く  

結果として、「速さ（セルフサービス）」と「守り（サプライチェーン信頼）」を同じ物語で説明できます。

## デプロイ上の注意（ハンズオン向け）

- OpenShift 上での利用が中心のストーリーが多い（マネージド OpenShift 上の検証も一般的）  
- コンポーネントは自己管理（セルフマネージド）が基本、という説明が多い  
- 本資料では特定クラスタの接続情報は扱わない

## 参考リンク（公開情報）

- [Red Hat Advanced Developer Suite](https://www.redhat.com/en/products/advanced-developer-suite)  
- [Components of RHADS](https://www.redhat.com/en/products/advanced-developer-suite/components)  
- [RHADS - software supply chain ドキュメント](https://docs.redhat.com/en/documentation/red_hat_advanced_developer_suite_-_software_supply_chain/)  

（リンク先は公開ページ。社内専用ドキュメントがある場合は、案内時に別途共有する。）
