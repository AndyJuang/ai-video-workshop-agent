> 本檔逐字取自工作坊「提示詞定稿 v9」（與學生講義 v10 相同，含全形標點與 [ ]）。標題中的「投影片 N 備註」是課堂簡報的頁碼，可以忽略。**[ ] 方括號裡的文字換成你們組的內容，方括號以外不要改。** 方括號裡現有的內容是示範主題「幼兒園的一天」，屬於**教學用模擬素材**。

## FFmpeg 四個指令：AI 底下在跑的指令（2026/11/17 在 FFmpeg 7.1 實測｜講義第 5 節）

```bash
ffmpeg -i S01_raw.mp4 -vf "scale=1920:1080:force_original_aspect_ratio=decrease,pad=1920:1080:(ow-iw)/2:(oh-ih)/2,setsar=1,fps=30" -c:v libx264 -pix_fmt yuv420p -an S01.mp4
```

```bash
ffmpeg -f concat -safe 0 -i list.txt -c copy merged.mp4
```

```bash
ffmpeg -i merged.mp4 -i narration.mp3 -map 0:v -map 1:a -c:v copy -c:a aac -shortest with_voice.mp4
```

```bash
ffmpeg -i with_voice.mp4 -vf "subtitles=subs.srt:force_style='FontName=Microsoft JhengHei,FontSize=28'" -c:v libx264 -pix_fmt yuv420p -c:a copy final.mp4
```
