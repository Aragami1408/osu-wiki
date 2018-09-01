# BanchoBot

![BanchoBot's user card](img/BanchoBot.jpg "BanchoBot's user card")

Banchobot là một bot trợ giúp người chơi trong chat bằng cách hiển thị thông tin rõ ràng và thông báo liên quan đến game. Nó được lập trình bởi [Echo49](/users/431) và là owner của [Bancho IRC](/wiki/Internet_Relay_Chat). BanchoBot thậm chí còn có cả profile cho chính nó: [osu! profile](/users/3) and [Tài khoản twitter](https://twitter.com/banchoboat)!

## Các lệnh

*Danh sách các dòng lệnh trong osu! client có thể tham khảo ở: [Chat Console](/wiki/Chat_Console#commands-list)*

Lệnh của BanchoBot có prefix là "!". Các lệnh này sử dụng được trong game và IRC. Chúng có thể dùng ở multiplayer chat và PM cho BanchoBot. Nếu là người dùng thường gửi message cho BanchoBot ở chat công cộng, người dùng còn lại sẽ không thấy nó, nhưng phản hồi chỉ có thể thấy trong PM.

Bạn vẫn có thể sử dụng `/bb` trong client để mở tab "BanchoBot" và gửi được các lệnh một cách nhanh chóng.

*Notice: lệnh `SEARCH` không được thêm vào đồng nghĩa nó không hoạt động được*

*Note: Việc tranh luận của người dùng là trường hợp không nhạy cảm, cũng như tên người dùng*

### HELP

```
!HELP
```

Hiện ra danh sách các lệnh có sẵn cho BanchoBot

#### Thí dụ cách dùng



```
pippi: !help
BanchoBot: Standard Commands (!COMMAND or /msg BanchoBot COMMAND):
BanchoBot: SEARCH <query>|next|prev
BanchoBot: WHERE <user>
BanchoBot: STATS <user>
BanchoBot: FAQ <item>|list
BanchoBot: REPORT <user> <reason> - call for an admin
BanchoBot: REQUEST [list] - shows a random recent mod request
BanchoBot: ROLL <number> - roll a dice and get random result from 1 to number(default 100)
```

### ROLL

```
!ROLL <number>
```

Rút ra một số bất kì từ 1 đến `<number>` (Mặc định là 100)

#### Thí dụ cách dùng

```
pippi: !roll 1000
BanchoBot: pippi rolls 109 point(s)
```

### STATS

```
!STATS <user>
```

Hiển thị thống kê về người dùng đã được nhập. Kết quả thống kê dựa vào chế độ chơi mà đang chơi và lần chơi cuối cùng

*Notice: BanchoBot sẽ không nói cho bạn biết chế độ chơi từ thống kê*

*Note: Nếu BanchoBot phản hồi đại loại như: `User not found` nếu user không chơi lần nào thậm chí user đó không tồn tại*

#### Thí dụ cách dùng

```
pippi: !stats peppy
BanchoBot: Stats for peppy:
BanchoBot: Store: 422,187,979 (#94718)
BanchoBot: Plays: 7149 (lv65)
BanchoBot: Accuracy: 87.29%
```

```
pippi: !stats Ephemeral:
BanchoBot: Stats for Ephemeral is Playing:
BanchoBot: Store: 2,384,155,536 (#33697)
BanchoBot: Plays: 14054 (lv96)
BanchoBot: Accuracy: 94.19%
```

### WHERE

```
!WHERE <user>
```

Hiển thị vị trí của user

*Notice: Lệnh này chỉ cho biết quốc tịch của user*

#### Thí dụ cách dùng

```
pippi: !where Ephemeral
BanchoBot: Ephemeral is in Australia
```

### FAQ

```
!FAQ <entry>
!FAQ list
```

Cung cấp thông tin đã được nhập. Bạn có thể dùng tham số `list` hiển thị tất cả các mục nhập có sẵn. Khi ban quan trị sử dụng nó ở channel công cộng, nó sẽ trả về đúng channel đó. Nếu là người dùng thường thì nó sẽ phản hồi ở BanchoBot private message.

#### Thí dụ cách dùng

```
pippi: !faq peppy
BanchoBot: peppy is the lead developer and indeed, the creator of osu! and handles most of the project himself.
```

```
Tama: 你好
Yuzu: !faq chinese
BanchoBot: 中文用户请点击 #chinese 以进入中文频道进行交流。
BanchoBot: #osu 是英文专属频道，如果接获此讯息后继续在 #osu 内以中文交谈，管理员有权利禁言。
Tama: ok
```

### REPORT

*Notice: Nếu bạn muốn report ban quản trị, hãy gửi mail cho [support@ppy.sh](mailto:support@ppy.sh)*

*Note: Bạn có thể dùng user card để report user đó*

```
!REPORT <user> <reason>
```


*Notice: Tên người dùng có dấu cách sẽ thay thế bằng dấu gạch dưới (`_`)*

Gửi report tới [Global Moderation Team](/wiki/Global_Moderation_Team) hoặc [Language Moderators](/wiki/Language_Moderators).

#### Thí dụ cách dùng

```
pippi: !report flyte spamming in #japanese
BanchoBot: Chat moderators have been alerted. Thanks for your help.
```

### REQUEST

```
!REQUEST
!REQUEST list
```

Gửi link tới một beatmap hiện tại từ yêu cầu của người quản lý. Bạn có thể dùng tham số `list` để lấy nhiều hơn một. Chọn link thì sẽ mở web hoặc osu!direct nếu bạn mua osu!supporter

#### Thí dụ cách dùng

```
pippi: !request
BanchoBot: HoneyWorks - Tokyo Summer Session feat. CHiCO by MrSergio
```