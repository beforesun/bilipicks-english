# 程程学英语

面向小学四年级、能读简单句但听说较弱的孩子的六周英语听说成长路线。基于 [BiliPicks](https://github.com/limin112/bilipicks) 改编，保留其 MIT 许可。网站不使用推荐算法，只展示家长选定的视频。

- 第 1 周：A–M，先看 26 字母音总览，再每天练 2–3 个字母。
- 第 2 周：N–Z，完成 A–Z 听辨与发音自测。
- 第 3 周：a/e/i/o/u 五个短元音，练 CVC 单词拼读及常见辅音组合。
- 第 4 周：问候、年龄等日常对话。
- 第 5 周：听问句、听短故事，抓关键词回答。
- 第 6 周：用三句英语复述绘本故事。

40 张视频卡中，26 个字母和 5 个短元音分集分别记录进度。字母歌用于听读和找词；字母音以完整讲解和家长示范为准。每天练习约 10 分钟，完成视频后再做本关口头任务。网页的进度只是手动记录，不会自动判断是否学会。家长请先试播视频；部分内容是转载，可能下架或变更。

打开 [网页学习版](https://beforesun.github.io/bilipicks-english/) 或 [电视版](https://beforesun.github.io/bilipicks-english/tv.html)。电视 App 安装包见仓库的 `android/release/程程学英语.apk`。它使用独立包名，可与原版 BiliPicks 同时安装，安装后显示名为「程程学英语」。电视版用方向键和确定键操作。

课程内容在 `data.js`。同一 BV 号的不同分集用独立 `id`，真实 BV 号保存在 `bvid`，`page` 指向分集。维护视频可运行 `python3 update.py --check`，添加视频用 `python3 update.py add BV号 --cat 分类 --age 9 --reason "推荐理由" --stage 关卡号 --note "本关作用"`。网页进度保存在设备本地，换设备不会同步。

Android 源码在 `android/`，其 `MainActivity.java` 指向本仓库的 GitHub Pages。构建参见 `android/README.md`。发布新版时需用同一签名密钥，否则必须先卸载旧版。
