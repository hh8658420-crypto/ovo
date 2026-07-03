最终版功能：
1. 同步开奖结果：同一个 room=VIP001 的所有设备使用同一倒计时、同一开奖结果、同一路单。
2. 同步下注金额：下注写入 Firebase 的 rooms/VIP001/clientBets，其他设备会同步显示下注总额和百分比。
3. 视频人物位置已下移，脸部更靠中间。

上传方式：
把本 ZIP 解压后，里面所有文件直接上传到 GitHub 仓库根目录。不要上传外层文件夹，不要只上传 index.html。

根目录应包含：
index.html
firebase-config.js
firebase-rules-demo.json
hj.mp4
hj_poster_small.jpg
README-上传说明.txt
README-最终上传说明.txt

Firebase Rules 测试规则：
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

测试链接示例：
https://hh8658420-crypto.github.io/ovo/?v=finalsync1&room=VIP001
