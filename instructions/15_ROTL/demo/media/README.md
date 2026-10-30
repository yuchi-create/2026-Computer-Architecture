# 15_ROTL/demo/media/

簡報與 Demo 用的動畫檔。由 [`demo/render_media.py`](../render_media.py) 產生,不需要手動編輯。

| 檔案 | 內容 |
|---|---|
| `rotl_encode.gif` / `.mp4` | 把 funct7、rs2、rs1、funct3、rd、opcode 組成 `0x00C5850B` |
| `make_test_all_passed.gif` / `.mp4` | `make test` 全數通過的畫面 |
| `m5_speedup.gif` / `.mp4` | ARM64 實機量測的加速比 |

重新輸出(需要 `ffmpeg`):

```bash
make media
```

這些檔案只用在簡報,不屬於 CP3 的評分內容。
