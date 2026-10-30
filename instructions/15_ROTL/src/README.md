# 15_ROTL/src/

原始碼依 Checkpoint 分成兩個目錄:

| 目錄 | 對應 Checkpoint | 內容 |
|---|---|---|
| [`c_baseline/`](c_baseline/README.md) | CP1 | C 參考實作、測試程式與 UBSan 反例 |
| [`rv32im/`](rv32im/README.md) | CP2–CP3 | RV32IM 組合語言、ChaCha20 / RC5 核心與自訂指令 |

建置與測試指令都在 `instructions/15_ROTL/` 執行,例如 `make test`、`make counts`、`make encode`。
