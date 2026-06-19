# img2-sd2-character-prompts V2

## 任務目的

`img2-sd2-character-prompts V2` 是用於把多張角色參考圖整理成 SD2 / Image2 可重複使用角色包的固定流程。本版以「翠花」11 張參考照片完成驗證，包含角色 profile、四份 prompt、四張圖卡與生成報告。

## V2 核心規則

- 每次新角色必須建立完整角色包。
- 每次新角色必須輸出 `CHARACTER_PROFILE.json`。
- 每次新角色必須保存原始參考圖到 `01_reference_images/`。
- 每次新角色必須輸出四份 prompt：主視覺角色卡、展示卡、角色設定圖卡、15 格人物展示卡。
- 每次新角色必須生成四張圖卡：主視覺角色卡、展示卡、角色設定圖卡、15 格人物展示卡。
- 不調用 API，不要求 `OPENAI_API_KEY`。
- 圖像生成使用 Codex 內建 image_gen 或使用者已登入的圖像生成工具。
- 舊檔不覆蓋；新版使用 `_v1`、`_v2`、`_v3` 等版本檔名。

## 使用素材

本次驗證角色：翠花 / CUIHUA。

來源資料夾：

```text
\\192.168.0.19\homes\pony6832\Pony's File\翠花\2026-05\
```

使用檔案：

```text
20260524_205447.jpg
20260531_205127.jpg
20260501_145107.jpg
20260523_175332.jpg
20260514_073525.jpg
20260522_234931.jpg
20260515_001529.jpg
20260503_133138.jpg
20260503_133214.jpg
20260502_165359.jpg
20260502_165337.jpg
```

## 翠花角色辨識特徵

- 名稱：翠花 / CUIHUA
- 種類：短毛棕金虎斑家貓
- 固定外觀：額頭深色 M 字紋、黑色虎斑條紋、杏金色圓眼、粉棕鼻、白下巴、淡奶油色口鼻、長白鬍鬚、大而直立的三角耳
- 固定配件：藍白圓鈴鐺吊牌
- 常見場景：淺藍毛巾或毯子、粉紅魚玩具、黑色網格切割墊、居家桌面或床鋪
- 氣質：慵懶、好奇、親近、愛玩、表情有戲

## 本地角色包位置

```text
C:\Users\pony6832\Documents\老馬的日常專案\角色包\CUIHUA_TABBY_CAT_V1
```

## 固定輸出結構

```text
CUIHUA_TABBY_CAT_V1/
  CHARACTER_PROFILE.json
  01_reference_images/
  02_character_cards/
    CUIHUA_TABBY_CAT_主視覺角色卡_v1.png
    CUIHUA_TABBY_CAT_展示卡_v1.png
    CUIHUA_TABBY_CAT_角色設定圖卡_v1.png
    CUIHUA_TABBY_CAT_15格人物展示卡_v1.png
  03_prompts/
    CUIHUA_TABBY_CAT_主視覺角色卡_prompt_v1.md
    CUIHUA_TABBY_CAT_展示卡_prompt_v1.md
    CUIHUA_TABBY_CAT_角色設定圖卡_prompt_v1.md
    CUIHUA_TABBY_CAT_15格人物展示卡_prompt_v1.md
  04_reports/
    生成報告_v1.md
```

## 執行流程

1. 讀取專案固定規則：
   - `img2-sd2-character-prompts_固定流程.md`
   - `生圖與Seedance2固定規則_v1.md`
2. 建立角色包資料夾：
   - `01_reference_images`
   - `02_character_cards`
   - `03_prompts`
   - `04_reports`
3. 複製參考圖到 `01_reference_images/`。
4. 建立 `CHARACTER_PROFILE.json`，鎖定角色外觀、配件、場景、可變與不可變特徵。
5. 產出四份可直接貼入 SD2 / Image2 的 prompt：
   - 主視覺角色卡 prompt
   - 展示卡 prompt
   - 角色設定圖卡 prompt
   - 15 格人物展示卡 prompt
6. 使用 Codex 內建 image_gen 生成四張圖卡。
7. 將生成圖複製到 `02_character_cards/`，保留固定檔名。
8. 更新 `04_reports/生成報告_v1.md`，記錄素材、prompt、生成圖路徑、檢查清單與備註。

## 四張圖卡要求

### 1. 主視覺角色卡

單一連貫真實攝影場景，優先鎖定角色身份與主視覺氣質。不做粗糙拼貼，不做商品廣告版型。

### 2. 展示卡

單一連貫展示場景，呈現角色全身、環境與常見道具。本次翠花展示卡包含淺藍毛巾、黑色網格切割墊與粉紅魚玩具。

### 3. 角色設定圖卡

排版型角色設定卡，包含正面、3/4、側面、紋路、細節、配件與色票。可有圖卡文字標籤，但需保持乾淨、簡短、可讀。

### 4. 15 格人物展示卡

固定 15 格，建議 5 欄 x 3 列。每格展現同一角色的不同角度、表情、局部細節、道具與場景互動。

## 固定負面 Prompt

```text
no text overlay, no subtitles, no watermark, no logo, no UI, clean frame, no readable brand logo, no product ad layout, no captions, no cartoon, no anime, no illustration, no CG render, no 3D render, no plastic fur, no unrealistic cat anatomy, no extra limbs, no deformed paws, no distorted face, no different cat, no different eye color, no long-haired breed, no dog-like face
```

## 翠花重跑強化 Prompt

若生成時角色漂移，追加：

```text
same cat identity, same brown-golden mackerel tabby markings, same dark M forehead marking, same amber-gold eyes, same pink-brown nose, same white chin, same blue-white round bell charm
```

若角色設定圖卡需要嚴格欄位，追加：

```text
Do not add extra sections beyond the requested layout.
```

若 15 格展示卡需要避免多格或少格，追加：

```text
exactly 15 numbered panels, 5 columns x 3 rows, do not create a 16th panel
```

## 本次生成結果

- `CUIHUA_TABBY_CAT_主視覺角色卡_v1.png`：已生成。
- `CUIHUA_TABBY_CAT_展示卡_v1.png`：已生成。
- `CUIHUA_TABBY_CAT_角色設定圖卡_v1.png`：已生成；版面包含額外的 `HOME ENVIRONMENT` 欄位，整體仍可作為角色設定圖卡。
- `CUIHUA_TABBY_CAT_15格人物展示卡_v1.png`：已生成，為正確 15 格展示卡。

## 驗收清單

- 參考圖已保存到 `01_reference_images/`。
- `CHARACTER_PROFILE.json` 已建立。
- 主視覺角色卡 prompt 已保存。
- 展示卡 prompt 已保存。
- 角色設定圖卡 prompt 已保存。
- 15 格人物展示卡 prompt 已保存。
- 主視覺角色卡圖像已保存。
- 展示卡圖像已保存。
- 角色設定圖卡圖像已保存。
- 15 格人物展示卡圖像已保存。
- 生成報告已更新。
- 固定流程中的「角色設定圖卡」與「15 格人物展示卡」皆已交付。

## 入倉紀錄

- 倉庫：`pony6832/img2-sd2-character-prompts`
- 流程名稱：`img2-sd2-character-prompts V2`
- 文件路徑：`docs/img2-sd2-character-prompts_V2.md`
- 日期：2026-06-19
