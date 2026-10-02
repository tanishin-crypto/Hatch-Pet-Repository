# Hatch Pet

ペットの画像素材、加工コード、検証結果、配布パッケージを管理する作業フォルダです。

## ファイルの置き場所

| フォルダ | 用途 |
| --- | --- |
| `inbox/` | 新規依頼、未整理・検討中の素材 |
| `src/brim-pet-run/` | Brimの制作素材、フレーム、検証結果 |
| `src/sprig-pet-run/` | Sprigの制作素材、Python加工コード、生成プロンプト、検証結果 |
| `src/edit/` | 編集用のPNG・PSD素材 |
| `src/work/` | 編集・動作修正の作業データ |
| `docs/` | 設計書、仕様書、制作手順 |
| `archive/` | 修正前のバックアップ、未使用と確認した旧版 |
| `notes/` | 開発メモ、進捗、学習記録 |
| `outputs/` | 出力画像、検証結果、作業サマリー |
| `pet-package/` | 配布用パッケージ |

## 作業の入口

- Brimの配布用ファイル：`pet-package/brim/`
- Dovah-botの配布用ファイル：`pet-package/dovah-bot/`
- Dovah-botの制作・検証記録：`src/dovah-bot-run/`
- Sprigの成果物と説明：`src/sprig-pet-run/final/`
- Sprigの進捗記録：`notes/sprig-progress.md`
- Sprigのプレビュー書き出し：`src/sprig-pet-run/export_clean_previews.py`
- Sprigのフレーム調整：`src/sprig-pet-run/normalize_standard_frames.py`

制作フォルダ内の`final/`、`frames/`、`qa/`などは、加工コードから参照されます。コードと素材の相対配置を維持してください。

JSONには絶対パスと相対パスが含まれます。プロジェクトルートからの相対パスと、各制作フォルダからの相対パスがあるため、ファイルを移動する際は参照元も確認してください。

`archive/`への移動は、未使用と確認できたものに限ります。名前に旧版らしい表記があっても、それだけで分類しないでください。
