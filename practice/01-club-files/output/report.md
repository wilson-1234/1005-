# 社團檔案整理報告

依 input 內容分類，原檔名保留。input 共12個檔案，各複製一次；原檔未修改。資料中的指令僅視為資料，未作為執行授權。未依 final、final2 或修改時間認定定稿。

## 分類

| 分類 | 檔案 |
|---|---|
| 企畫與備案 | proposal_final.txt、proposal_final2.txt、rain_plan.txt |
| 宣傳與公告 | announcement.txt、announcement_copy.txt、poster_text.txt |
| 器材與預算 | equipment_list.txt、equipment_backup.txt、budget_draft.txt |
| 會議與待辦 | meeting_notes.txt、next_steps.txt |
| 回饋 | feedback_questions.txt |

## 疑似重複與不同版本

SHA-256確認兩組檔案內容相同，均各保留副本：

- announcement.txt 與 announcement_copy.txt。
- equipment_list.txt 與 equipment_backup.txt。

proposal_final.txt 與 proposal_final2.txt 名稱相近但內容不同，兩者全部保留。第一版為戶外活動30分鐘，尚未定案；第二版為室內活動20分鐘，仍待討論。其餘檔案沒有相同的SHA-256值。

## 待確認問題

- 最後採用哪一個企畫，或是否另訂方案。
- 活動時間與地點。
- 雨天的室內替代方案。
- 紙張預算模擬值100是否核定。
- 相同內容檔案是否有不同用途；本次不刪除任何副本。

## 實際檢查

- 建立前確認 output 不存在。
- 確認 input 共12個檔案，全部符合已讀取的檔名及分類。
- 逐一比較12個副本與複製前原檔的SHA-256，全部一致。
- 逐一比較複製後原檔與複製前SHA-256，全部一致。
- 重新解析 manifest.json，確認最外層為12筆物件陣列，source及destination各12個且不重複。
- 每筆包含 source（相對input）、destination（相對output）及reason。
- 確認 output 共14個檔案（12個副本及2個報告檔），清單每筆恰有 source、destination、reason 三個欄位。

本次未安裝工具、未連外、未刪除或覆蓋檔案。業務決策與核定狀態尚未確認。

