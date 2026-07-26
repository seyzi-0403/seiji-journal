# seiji-journal

緒方聖士の音声ジャーナル → Claude記憶 自動反映パイプライン。

- `journal/`: iPhone Shortcuts から直接投稿される、日々の音声ジャーナルの文字起こし（Markdown）
- `memory/`: 週次のクラウドエージェントが `journal/` を読んで抽出した、恒久的な記憶ノート（`journal-` prefixのファイルのみ）。ローカルの `~/.claude/projects/-Users-ogataseiji-Claude/memory/` に SessionStart フックで同期される。
- `memory/.journal_processed.log`: 処理済みジャーナルファイル名の一覧（重複処理防止用）
