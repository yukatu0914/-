<div align="center">

<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

  <h1>Built with AI Studio</h2>

  <p>The fastest path from prompt to production with Gemini.</p>

  <a href="https://aistudio.google.com/apps">Start building</a>

</div>

## 毎週月曜日9時のAIレポート出力

`ai_monday_report.py` はAIに関する記述式の情報を5件出力します。以下のcron設定を使用すると、毎週月曜日の9:00に自動実行されます。

```cron
0 9 * * 1 /usr/bin/env python3 /workspace/-/ai_monday_report.py >> /workspace/-/ai_monday_report.log 2>&1
```

ローカルで動作確認する場合:

```bash
python3 ai_monday_report.py
```
