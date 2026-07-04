# TL ウォーターマーク強化ツール

Throne and Liberty のギア強化（Watermark / ドロップ確率）を誰でも使えるシンプルな Web ツールとして提供します。

## 機能

- **計算タブ**: 武器 / 防具 / アクセサリーの現在 IL を入力して WM を算出。次ドロップ確率・弱いカテゴリをハイライト。
- **シミュレーションタブ**: モンテカルロ法で目標 WM 到達までの平均ドロップ数・分布を推定。
- **確率表タブ**: 全 WM (21–80) のドロップ確率ヒートマップ。

## データ出典

- Google Sheets: *How to Level Up Gear by Aragon & Kninebeat*（最終更新 2026-07-04）
- 解説動画: https://youtu.be/tJql3gCP4WY

## 注意事項

- シミュレーションのドロップカテゴリは均等 1/3 割り当てを前提にしています。実際のゲーム内確率と異なる可能性があります。
- データは 2026-07-04 時点のものです。ゲームアップデートにより変更される場合があります。

## デプロイ

Cloudflare Pages に直接アップロード:

```bash
npx wrangler pages deploy . --project-name tl-watermark-tool
```
