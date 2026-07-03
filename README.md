# OVO VIP 联机同步版

上传方式：把本文件夹里的 index.html、firebase-config.js、firebase-rules-demo.json 上传到 GitHub 仓库根目录，覆盖旧文件。

打开测试：
https://hh8658420-crypto.github.io/ovo/?v=vip-sync-ui-1&room=VIP001

本版修复：
- 每个页面会话使用独立玩家 ID，同一手机/同一浏览器开两个页面测试也不会互相覆盖下注。
- 下注数字走 rooms/{房间}/clientBets/{玩家会话ID} 实时同步。
- 开奖/倒计时/开奖记录走 rooms/{房间}/state 实时同步。
- 页面样式改成接近 baccarat-vip final 的移动端布局。

注意：这是前端模拟游戏，不含真钱支付。
