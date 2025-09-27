# 🎦 daDashCam.Player

<img width="320" height="320" alt="dadashcam-player" src="https://github.com/user-attachments/assets/ff7dec7c-682c-4196-9fec-1d217cdc765a" />

`daDashCam Player の配布用リポジトリです`

## 概要 / Overview

`daDashCam`が操作を「記録」するツールであるのに対し、`daDashCam Player`はその記録を「分析」するためのツールです。

「特定の操作をしたらPCが重くなった」「バッチ処理中にCPU使用率がどう変化したか知りたい」といった疑問に答えるため、本プレイヤーは動画のタイムラインとパフォーマンスデータを完全に同期させます。動画を再生・シーク・一時停止すると、その時点でのCPU使用率、メモリ使用量、ディスクI/Oがグラフ上にリアルタイムでプロットされ、パフォーマンスのボトルネックやシステムへの影響を直感的に把握できます。


<img width="650" height="630" alt="capture_2025-9-22_16-02-53" src="https://github.com/user-attachments/assets/99d07487-b859-416c-ab4a-8ff0141be28a" />

## 主な特徴 / Features

-   **📊 ログと動画の完全同期 (Perfect Sync of Video & Logs)**
    -   動画の再生ヘッドに合わせて、CSVに記録されたパフォーマンスデータ（CPU, メモリ, ディスクI/O）がグラフに描画されます。
    -   動画をシークするとグラフも追従するため、気になる時点のパフォーマンスを即座に確認できます。

-   **📈 パフォーマンスの可視化 (Performance Visualization)**
    -   [Chart.js](https://www.chartjs.org/) を利用した美麗なグラフで、システムリソースの推移を視覚的に分かりやすく表示します。
    -   CPU・メモリ使用率とディスクI/Oをそれぞれ別のグラフで表示し、詳細な分析をサポートします。

-   **🔍 フレーム単位の精密な分析 (Frame-by-Frame Analysis)**
    -   `▶` `❚❚` `⏪` `⏩` といった基本的な再生コントロールに加え、**1コマ送り・1コマ戻し**機能を搭載。
    -   パフォーマンスが急上昇したまさにその「瞬間」、画面上で何が起きていたのかをフレーム単位で正確に特定できます。

-   **🛠️ 便利なユーティリティ (Convenient Utilities)**
    -   **スクリーンショット**: 気になる瞬間をワンクリックで画像（.png）として保存できます。
    -   **MP4変換**: `daDashCam`で録画したWebM動画を、より汎用性の高いMP4形式に変換して出力できます。

## ユースケース / Use Cases

-   **開発者 / QAエンジニア**
    -   アプリケーションのパフォーマンステストにおいて、特定の操作がシステムリソースに与える影響を分析する。
    -   「操作が重い」というバグ報告に対し、動画とデータを突き合わせて原因を調査する。

-   **システム管理者 / ITサポート**
    -   ユーザーから提供された録画データをもとに、PCの不調や特定ソフトウェアの問題をリモートで診断する。

-   **パワーユーザー**
    -   新しいソフトウェアを試す際に、バックグラウンドでどれだけのリソースを消費しているかを確認する。

## インストール / Installation

最新バージョンは、[リリースページ](https://github.com/1010-junji/BR.daDashCam.Player/releases)からダウンロードできます。
`.webm`ファイルとの関連付けをサポートするインストーラー版 (`.exe`)と、ポータブル版 (`.zip`)を用意しています。

## クイックスタート / Quick Start

1.  `daDashCam`で録画した `.webm` ファイルと、同時に出力された `.csv` ファイルを同じフォルダに配置します。
2.  本アプリケーションを起動し、`[動画（webm）を選択]`ボタンから `.webm` ファイルを開きます。
3.  または、インストーラー版を導入している場合、`.webm`ファイルをダブルクリックするだけで本プレイヤーが起動し、動画とCSVが自動的に読み込まれます。
  
詳細な使い方はリリースページ内に同梱された **ユーザーマニュアル** をご覧ください。

## daDashCam

daDashCam 入手はこちらから。👉 https://github.com/1010-junji/BR.daDashCam

<img width="120" height="120" alt="dashcam" src="https://github.com/user-attachments/assets/6ec1239e-e490-478f-ab1d-e2bfee3fa75e" />  


## コントリビュート / Contributing

バグ報告、機能提案、プルリクエストを歓迎します！
何かお気づきの点があれば、お気軽に[Issue](https://github.com/1010-junji/BR.daDashCam.Player/issues)を立ててください。
