# OVO 联机同步修复完整版

直接把本压缩包里的文件上传到 GitHub 仓库根目录即可。

修复点：

- 开奖结果通过 `rooms/{room}/state` 同步。
- 下注数字通过 `rooms/{room}/clientBets/{clientId}` 同步。
- 下注数字监听和开奖记录监听互不覆盖。
- 远端玩家下注只更新数字，不生成筹码堆。
- 支持 `?room=VIP001` 房间参数。

测试链接示例：

`https://hh8658420-crypto.github.io/ovo/?v=complete-sync-1&room=VIP001`

如果你上传后还看到旧页面，请修改 URL 里的 `v=` 参数强制刷新缓存。
