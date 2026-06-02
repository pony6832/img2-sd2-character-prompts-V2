# LUNA XIA - 20 格人物展示分鏡腳本

## Purpose

這份文件用來生成一張符合 LUNA XIA 角色卡設定的 20 格人物展示分鏡圖，並提供可拆成 Seedance 2.0 影片測試的逐格 Prompt。

核心原則：

- 保持同一角色身份：LUNA XIA，月光包廂系都市夢幻歌姬。
- 保持同一組身份錨點：長直棕紅髮、透明/銀框眼鏡、白色斜肩服、銀色有線耳機、銀色有線麥克風、粉紫燈。
- 20 格混合全身、半身、近臉、手部、道具、背面、動作與情緒。
- 生成圖卡時不要手機 UI、直播留言、狀態列、平台標誌或字幕。

## 20 格 Layout

1. **Full Body Hero** - 全身正面站姿，白色斜肩服，銀色麥克風垂在身側，粉紫背光。
2. **3/4 Lounge Pose** - 3/4 坐姿，靠在米色沙發，麥克風靠近唇邊。
3. **Side Singing Profile** - 側臉唱歌，耳機線清楚垂落，眼鏡反光。
4. **Kneeling Stage Pose** - 低角度舞台姿勢，白色布料自然垂落，麥克風線延伸到畫面外。
5. **Calm Portrait** - 正面半身，平靜凝視鏡頭，粉紫光打在臉頰。
6. **Soft Smile Portrait** - 輕微微笑，透明/銀框眼鏡戴在臉上。
7. **Dreamy Gaze** - 夢幻眼神，看向鏡頭外，長髮覆在肩上。
8. **Focused Singing** - 麥克風貼近唇邊，嘴型自然，不誇張張口。
9. **Eye Close-Up** - 眼睛與眼鏡特寫，細緻睫毛、粉紫反光。
10. **Lip Close-Up** - 唇部與麥克風網頭局部特寫，柔和光澤。
11. **Microphone Grip** - 手握銀色麥克風特寫，手指自然，金屬網頭清楚。
12. **Cable Touch** - 手指輕碰麥克風線，耳機線與麥克風線形成細緻線條。
13. **In-Ear Monitor Detail** - 耳機與耳環特寫，銀色線材垂落。
14. **Glasses On Head Detail** - 眼鏡推到頭頂，頭髮髮根蓬鬆，仍維持角色臉型。
15. **White Outfit Fabric** - 白色斜肩上衣布料特寫，柔軟褶皺與肩線。
16. **Back Hair View** - 背面髮型與耳機線，長直棕紅髮自然垂落。
17. **Over Shoulder Look** - 回眸半身，深色木牆與米色沙發背景。
18. **Stage Light Silhouette** - 粉紫光剪影，麥克風線與白色服裝輪廓明確。
19. **Direct Intimate Reach** - 近距離伸手向鏡頭，另一手握麥克風，景深強。
20. **Final Performance Wide** - 小型私密舞台全景，角色獨自站在粉紫光中唱歌。

## Image2 Master Prompt

```text
Create a 20-panel cinematic semi-realistic character storyboard contact sheet for an original character named LUNA XIA, moonlight livehouse vocalist and urban dream-pop idol. The image should match the structure of a professional 20-frame character display board: one square canvas, thin white gutters between panels, no large title text, no labels, no phone UI, no livestream comments.

Character identity lock: LUNA XIA is a young adult female singer with a delicate oval face, smooth fair skin, soft cheek volume, glossy natural pink lips, subtle winged eyeliner, warm peach-pink makeup, expressive calm eyes, and long straight warm auburn-brown hair with softly lifted crown and loose face-framing strands. She wears thin clear or silver rim glasses, a white asymmetrical off-shoulder wrap-style top with soft fabric folds, silver wired in-ear monitors with visible cable lines, small metallic earrings, a delicate silver necklace, and holds a metallic silver wired microphone with mesh grille and dark cable connector.

Visual style: cinematic semi-realistic idol concept art, intimate private karaoke lounge and small livehouse atmosphere, beige sofa, dark wood wall panels, soft pink-magenta and violet neon glow, shallow depth of field, high-detail hair strands, realistic skin texture, natural hand motion, polished music-video composition. Color palette: pearl white, warm auburn brown, silver, champagne beige, smoky charcoal, soft pink, magenta, violet.

20-panel content, arranged as a balanced contact sheet:
1 full-body front hero pose with microphone,
2 3/4 lounge sitting pose,
3 side singing profile with visible earphone cable,
4 low kneeling stage pose with microphone cable,
5 calm front portrait,
6 soft smile portrait,
7 dreamy gaze portrait,
8 focused singing portrait,
9 eye and glasses close-up,
10 lips and microphone grille close-up,
11 hand gripping silver microphone close-up,
12 fingers touching microphone cable close-up,
13 in-ear monitor and earring detail,
14 glasses pushed onto head hair detail,
15 white off-shoulder fabric detail,
16 back hair and cable view,
17 over-shoulder look,
18 pink-violet stage light silhouette,
19 intimate reaching hand toward camera with microphone in the other hand,
20 final wide performance shot on a small private stage.

Keep the same character across all 20 panels. Keep the same auburn-brown hair, clear/silver glasses, white off-shoulder outfit, silver wired earphones, silver microphone, and pink-violet lighting. Make the panel composition varied like a cinematic storyboard/reference sheet, with full body, medium shots, close-ups, detail inserts, and action poses.

Avoid: phone screenshot, app status bar, livestream UI, comments, Chinese text, subtitles, logos, watermark, extra characters, different outfit, black outfit, short hair, missing glasses, missing earphones, wireless microphone, broken hands, extra fingers, distorted mouth, over-smoothed plastic face, chibi style, exaggerated anime comedy.
```

## Seedance 2.0 Identity Block

Use this same block before every panel prompt.

```text
@Image1 identity lock: LUNA XIA, a young adult moonlight livehouse vocalist and urban dream-pop idol, soft-spoken, dreamy, elegant, quietly confident. She has a delicate oval face, smooth fair skin, soft cheek volume, glossy natural pink lips, subtle winged eyeliner, warm peach-pink makeup, expressive calm eyes, and long straight warm auburn-brown hair with a softly lifted crown and loose face-framing strands.

Keep her exact styling consistent: thin clear or silver rim glasses, white asymmetrical off-shoulder wrap-style top with soft fabric folds, silver wired in-ear monitors with visible cable lines, small metallic earrings, delicate silver necklace, and a silver handheld wired microphone as her signature prop. The microphone remains full size and metallic silver throughout the shot, with a visible mesh grille and dark cable connector.

Visual style: cinematic semi-realistic idol character animation, intimate karaoke lounge atmosphere, dream-pop live performance mood, soft beauty lighting, pink-magenta and violet neon glow, dark wood wall panels, beige sofa, shallow depth of field, high-detail hair strands, realistic skin texture, natural hand motion, polished music-video composition. Color palette: pearl white, warm auburn brown, silver, champagne beige, smoky charcoal, soft pink, magenta, violet.
```

## Seedance 2.0 Panel Prompts

Append one panel prompt at a time after the identity block.

1. `Vertical full-body shot, LUNA XIA stands alone in a private livehouse room, holding the silver wired microphone at her side, white off-shoulder outfit glowing under pink-violet light, slow camera push-in, 9:16.`
2. `Vertical medium shot, LUNA XIA sits on a beige karaoke lounge sofa in a relaxed 3/4 pose, microphone near her lips, dark wood wall softly blurred behind her, subtle camera dolly forward, 9:16.`
3. `Side profile close-up, LUNA XIA sings softly into the silver wired microphone, earphone cable visible along her cheek and neck, pink light reflected on her clear glasses, static camera, 9:16.`
4. `Low angle medium shot, LUNA XIA kneels on a small stage while holding the microphone cable loosely, white fabric folds naturally, violet backlight creates a soft silhouette, slow tilt up, 9:16.`
5. `Front portrait shot, LUNA XIA looks calmly into the camera with the microphone below frame, subtle breathing motion, pink-magenta light across her cheeks, 9:16.`
6. `Close-up portrait, LUNA XIA gives a restrained soft smile behind clear silver rim glasses, microphone mesh barely visible at the bottom of frame, static camera, 9:16.`
7. `Dreamy medium close-up, LUNA XIA looks slightly off camera as if listening to music in her earphones, long auburn hair over both shoulders, slow camera push-in, 9:16.`
8. `Focused singing close-up, LUNA XIA holds the microphone close to her lips and sings with small natural mouth movement, shallow depth of field, 9:16.`
9. `Extreme close-up of LUNA XIA's eyes behind clear silver rim glasses, pink-violet reflections on lenses, natural blink once, static macro shot, 9:16.`
10. `Extreme close-up of LUNA XIA's glossy lips near the silver microphone grille, soft breath movement only, cinematic macro shot, 9:16.`
11. `Close-up of LUNA XIA's hand gripping the metallic silver wired microphone, fingers natural and relaxed, mesh grille and dark connector visible, slow rack focus, 9:16.`
12. `Close-up of LUNA XIA's fingers lightly touching the microphone cable, silver earphone cable also visible, pink light on fingertips, static macro shot, 9:16.`
13. `Detail close-up of LUNA XIA's silver wired in-ear monitor and small metallic earring, auburn hair strands moving gently, shallow focus, 9:16.`
14. `Hair and glasses detail, LUNA XIA has clear silver rim glasses pushed onto her head, softly lifted crown and loose strands visible, slow side camera move, 9:16.`
15. `Costume detail close-up, white asymmetrical off-shoulder fabric folds catch pink-violet light, silver necklace and earphone cable crossing softly, static camera, 9:16.`
16. `Back hair view, LUNA XIA faces away slightly, long straight auburn-brown hair falls down her back, earphone cable visible, soft lounge background, slow camera drift, 9:16.`
17. `Over-shoulder medium shot, LUNA XIA turns back toward the camera with calm dreamy eyes, microphone held at chest height, dark wood wall and beige sofa behind, 9:16.`
18. `Silhouette shot, LUNA XIA stands in pink-violet stage light holding the wired microphone, cable line visible against a smoky dark background, gentle camera sway, 9:16.`
19. `Intimate close-up, LUNA XIA reaches one hand gently toward the camera while holding the silver wired microphone in the other hand, strong depth of field, slow push-in, 9:16.`
20. `Wide vertical performance shot, LUNA XIA stands alone on a small private livehouse stage and sings softly into the microphone, violet light blooms behind her, polished music-video atmosphere, 9:16.`

## Universal Negative Prompt

```text
Negative prompt: no face drift, no changing facial structure, no changing hair color, no short hair, no different hairstyle, no missing glasses, no thick black glasses, no missing wired earphones, no missing microphone, no wireless microphone, no microphone morphing, silver wired microphone remains full size and unchanged throughout the shot, no different outfit, no black outfit, no school uniform, no fantasy armor, no extra jewelry overload, no broken hands, no extra fingers, no fused fingers, no warped fingers, no warped microphone grip, no distorted lips, no exaggerated mouth movement, no teeth distortion, no plastic skin, no over-smoothed doll face, no chibi style, no exaggerated anime comedy, no text overlays, no phone UI, no livestream comments, no app icons, no logo, no subtitles, no crowded scene, no extra main characters, no heavy camera shake, no fast camera spin.
```
