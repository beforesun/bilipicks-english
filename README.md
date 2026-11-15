# 程程学英语

面向小学四年级、能读简单句但听说较弱的孩子的四周英语听说成长路线。基于 [BiliPicks](https://github.com/limin112/bilipicks) 改编，保留其 MIT 许可。网站不使用推荐算法，只展示家长选定的视频。

- 第 1 周：自然拼读，听声音、敢开口。
- 第 2 周：日常对话，能问候、问年龄。
- 第 3 周：短句听力，能听问题并回答。
- 第 4 周：绘本表达，能用三句话讲小故事。

每周两段指定分集，每天练习约 10 分钟。看完视频后做口头任务；网页的进度只是手动记录，不会自动判断是否学会。家长请先试播视频。部分视频是转载，可能下架或变更。

打开 [网页学习版](https://beforesun.github.io/bilipicks-english/) 或 [电视版](https://beforesun.github.io/bilipicks-english/tv.html)。电视 App 安装包见仓库的 `android/release/程程学英语.apk`，安装后显示名为「程程学英语」。电视版用方向键和确定键操作。

课程内容在 `data.js`。维护视频可运行 `python3 update.py --check`，添加视频用 `python3 update.py add BV号 --cat 分类 --age 9 --reason "推荐理由" --stage 关卡号 --note "本关作用"`。网页进度保存在设备本地，换设备不会同步。

Android 源码在 `android/`，其 `MainActivity.java` 指向本仓库的 GitHub Pages。构建参见 `android/README.md`。发布新版时需用同一签名密钥，否则必须先卸载旧版。
