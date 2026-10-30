# report/figures/evidence/

在 `instructions/15_ROTL/` 執行 `make` 的終端機截圖與完整輸出(`.log`)。每張截圖第一行是執行時間、電腦、作業系統與 git commit。

- 執行環境:MacBook Air、macOS 27.0.1、Apple clang、`riscv64-elf-gcc (GCC) 16.2.0`、Python 3
- 執行日期:2026-10-30,commit `502f922`

| 檔案 | 指令 | 內容 | 結果 |
|---|---|---|---|
| `1_test-c.png` / `.log` | `make test-c test-ubsan` | CP1:16 組測資、69,000 次交叉比對、2,000 組性質檢查,再用 UBSan 跑一次 | ALL PASS,UBSan 無未定義行為 |
| `2_test-py.png` / `.log` | `make test-py` | CP2 / CP3:在 RV32IM 模擬器上驗證四個版本與兩個核心,並比對組譯器與 Python 編碼器的機器碼 | 22 個測試全部 OK |
| `3_counts.png` / `.log` | `make counts` | CP2 / CP3:重新產生指令數表 1–3 | 與 [`instruction_counts.md`](../instruction_counts.md) 相同 |
| `4_encode.png` / `.log` | `make encode` | CP3:三個範例的機器碼 | 與 CP3.md §2.4 相同 |

指令由 Claude Code 在組員的電腦上執行並截圖。
