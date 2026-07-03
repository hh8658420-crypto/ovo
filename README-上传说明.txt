新仓库上传说明

1. 新建公开仓库：baccarat-vip
2. 解压本 ZIP。
3. 不要上传外层文件夹，也不要上传 ZIP。
4. 把下面 5 个文件直接上传到仓库根目录：
   - index.html
   - firebase-config.js
   - firebase-rules-demo.json
   - hj.mp4
   - hj_poster_small.jpg
5. GitHub Pages 设置：main / /(root)
6. 等 Actions / Pages 变成绿色对勾后再打开：
   https://hh8658420-crypto.github.io/baccarat-vip/?v=newrepo1&room=VIP001

联机状态看页面顶部“联机诊断”：
- SDK实时同步中：Firebase 联机成功
- REST创建房间成功：备用联机成功
- Permission denied / 403：Firebase Realtime Database 规则没开写入
- 还是没有“联机诊断”：新仓库没有部署到这个版本

Firebase Realtime Database 测试规则：
{
  "rules": {
    "rooms": {
      "$roomId": {
        ".read": true,
        ".write": true
      }
    }
  }
}
