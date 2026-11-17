# ② 圖片生成

**目標**：做出角色前後一致的分鏡圖（S01.png…），加上影片縮圖；需要海報時一併做海報插圖。

**輸入**：總腳本第 ④ 部分（YAML 固定區塊＋每格 shot／action／scene）、第 ⑥ 部分（縮圖）、第 ⑦ 部分（海報主視覺）。

**用的提示詞**：[P2 分鏡圖 YAML 整理](../prompts/P2-storyboard-image-yaml.md)、[YAML 範例](../prompts/YAML-examples.md)、[P3 海報版面與插圖](../prompts/P3-poster.md)。

**預設工具（用手邊帳號能用的就好）**

| 工具 | 適合做什麼 |
|---|---|
| ChatGPT（圖片功能） | 在對話裡產生圖片，可選取局部再用文字修改；可指定畫面比例 |
| Google Gemini（Nano Banana 圖片模型） | 產生與編輯圖片；可上傳參考圖維持角色一致 |
| Canva（AI 圖片生成） | 產生插圖後直接排成海報、縮圖 |
| Adobe Firefly | 文字生圖，可用參考圖，附編輯工具 |

**步驟**

1. 從下方「風格關鍵字」選 1 個風格，寫進 YAML 的 `style:`。可以先用同一格試 2–3 個詞，全組投票再定案。
2. 先做一張**角色定裝圖**（滿意的角色全身圖），之後產圖時當參考圖上傳，並寫「保持角色外觀與參考圖相同」。
3. 每一格用 P2 整理：固定區塊一字不差，只改 shot、action、scene 三欄。
4. 產圖；不滿意一次只改一個地方，不要整段重寫。
5. 依鏡號存檔：S01.png、S02.png…；縮圖、海報插圖另外命名。

**YAML 只是排得比較整齊的文字，不是任何工具的專用格式。** 工具產出的畫面怪怪的，就改用 P2 同時產生的「文字版」。

**AI 圖片中的中文字常常會出錯**：分鏡圖、縮圖、海報插圖都請 AI「不要出現文字」，標題和說明之後在 Canva、PowerPoint 或剪輯軟體裡自己打。

### 風格關鍵字（一組選一個）

極簡 Minimalism ★｜繁複 Maximalism｜未來感 Futuristic｜向量插畫 Vector art ★｜拼貼 Collage art ★｜復古 Retro｜賽博龐克 Cyberpunk｜普普藝術 Pop art｜玻璃擬態 Glassmorphism｜黏土風 Clay style ★｜像素 Pixel art｜雜誌編排 Editorial｜千禧風 Y2K｜瑞士設計 Swiss design｜超現實 Surreal｜波希米亞 Bohemian｜維多利亞 Victorian｜塗鴉 Graffiti｜極光漸層 Aurora｜手寫風 Handwritten ★

（★ 比較適合幼教主題、也好上手。一組只選 1 種，分鏡圖、縮圖、海報插圖都照抄同一句。）

**海報（如果這組也要做海報）**：海報呈現結構、影片負責敘事。三原則：一個主訊息、三個區塊、圖比字多。用 P3 規劃版面。

**產出檔案**

- `images/角色定裝圖.png`
- `images/S01.png`、`images/S02.png`…（依鏡號）
- `images/縮圖.png`、`images/海報插圖_*.png`（需要時）
- 每張圖用過的提示詞記進 `project-log.md`

**關卡檢查表**

- □ 每一個鏡號都有圖
- □ 角色前後一致（同一段固定區塊、同一張定裝圖）
- □ 圖中沒有亂碼文字
- □ 沒有真實人物、名人、品牌商標、卡通角色；沒有寫「模仿某位畫家或繪本作者的風格」
- □ 角色用插畫風格，沒有寫實的兒童照片
