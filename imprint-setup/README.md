# imprint-setup

放給 imprint（claude-imprint）用的、已經換成 ombre 記憶的設定檔。

## cron-mcp-full.json

把 ombre 當記憶、保留 imprint 的 Telegram 發訊息與工具 MCP。

**怎麼用：** 裝好 claude-imprint 後，用這份**覆蓋掉** repo 根目錄的 `cron-mcp-full.json`：

```bash
cp imprint-setup/cron-mcp-full.json <claude-imprint 目錄>/cron-mcp-full.json
```

> 注意：`heartbeat.py` 是動態組 MCP 設定的，不吃這個檔。要讓主動關心也走 ombre，得另外改 `packages/imprint_heartbeat/heartbeat.py` 裡組記憶 MCP 的那段——卡住就把檔案貼回來。
