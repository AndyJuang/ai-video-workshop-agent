# 提示詞索引（P1–P6）

所有提示詞都逐字取自工作坊講義，編號不變。用法：複製 ```text``` 區塊 → 把 [ ] 換成你們組的內容 → 貼給 AI。方括號以外的文字不要改。

| 編號 | 階段 | 用途 | 檔案 |
|---|---|---|---|
| 示範素材 | ① | 「幼兒園的一天」虛構情境（教學用模擬素材） | [00-sample-material.md](00-sample-material.md) |
| P1 | ① 腳本創作 | 萬用反向提示詞：讓 AI 先訪問你，再寫九個部分的總腳本 | [P1-master-script.md](P1-master-script.md) |
| P2 | ② 圖片生成 | 把固定區塊＋一格分鏡整理成 YAML 與文字版產圖提示詞 | [P2-storyboard-image-yaml.md](P2-storyboard-image-yaml.md) |
| YAML 範例 | ② 圖片生成 | 「固定的不動，只改這格」的兩個範例（教學用模擬素材） | [YAML-examples.md](YAML-examples.md) |
| P3 | ② 圖片生成 | 海報版面與插圖提示詞 | [P3-poster.md](P3-poster.md) |
| P4 | ③ 生成影片 | 圖生影片：一個動作＋一種運鏡，標準版與保守版 | [P4-image-to-video.md](P4-image-to-video.md) |
| P4-2 | ③ 生成影片（進階 C） | NotebookLM（現名 Gemini Notebook）說明影片的自訂提示詞 | [P4-2-notebooklm-video-overview.md](P4-2-notebooklm-video-overview.md) |
| P5 | ④ AI 配音 | 配音稿（停頓、加重、語氣）＋AI 語音指示 | [P5-voiceover.md](P5-voiceover.md) |
| P6-1 | ⑤ AI 剪輯（進階） | 讓能讀寫資料夾的 AI 助理建資料夾、檢查／安裝工具（先問再裝） | [P6-1-setup.md](P6-1-setup.md) |
| P6-2 | ⑤ AI 剪輯（進階） | 風格參考：參考就好，不要照抄 | [P6-2-style-reference.md](P6-2-style-reference.md) |
| P6-3 | ⑤ AI 剪輯（進階） | 剪輯原片：先給剪輯計畫，同意後才剪 | [P6-3-edit.md](P6-3-edit.md) |
| 特效範例 | ⑤ AI 剪輯 | 請 AI 做一個特效的寫法 | [FX-effect-request-example.md](FX-effect-request-example.md) |
| FFmpeg | ⑤ AI 剪輯 | AI 底下在跑的四個指令（說明見 [workflow/05-edit-and-sound.md](../workflow/05-edit-and-sound.md)） | [FFmpeg-commands.md](FFmpeg-commands.md) |

每個提示詞都依同一個結構寫：**角色目標／輸入／步驟／限制／輸出格式／自我檢查**。
