# 截图风格 DB 真人联机百家乐

这是基于你发的截图重新做的移动端页面版本，已经接入现有 Firebase 联机同步。

上传方法：
1. 解压 ZIP。
2. 把 index.html、firebase-config.js、firebase-rules-demo.json 上传到 GitHub 仓库根目录。
3. 覆盖旧文件并 Commit。
4. 打开：
   https://hh8658420-crypto.github.io/ovo/?v=screenshot-style-online-1&room=VIP001

说明：
- 不包含视频文件；页面会尝试读取仓库里的 hj.mp4 / hj_poster_small.jpg。没有视频时会显示赌场色调占位背景。
- 倒计时 15 秒，到 0 不管有没有下注都会自动发牌。
- 发牌和开牌是一张一张慢慢显示。
- 补牌显示在闲/庄对应方框内。
- 开完奖后自动进入下一轮并隐藏上一轮牌。
- 下注金额、百分比、倒计时、开奖和路单走同房间同步。
- 筹码为模拟筹码，不含支付、充值、提现。
