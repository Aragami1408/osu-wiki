# Độ chính xác  

Độ chính xác (DCX) là thước đo có mang tính nhất quán đối với người chơi. Có tất cả ba kiểu ĐCX. Một trong số đó phụ thuộc vào số điểm nhận được trong một beatmap. Phần khác là DCX tổng thể của người chơi cho phép người chơi có điểm số tốt hơn. Sau đó, độ chính xác của người chơi [pp](/wiki/pp) được dựa vào điểm kết quả của người chơi.

## Các chế dộ game

### ![](/wiki/shared/mode/osu.png) osu!standard

![Accuracy = (50 \* number of 50s + 100 \* number of 100s + 300 \* number of 300s) / 300(number of 0s + number of 50s + number of 100s + number of 300s)](img/accuracy_standard.png)

Trong chế dộ standard, DCX được tính bằng cách lấy điểm nhận được chia cho điểm tối đa.

Bảng dưới biểu thị tính DCX đối với một note được hit: 


```
300 -> 300 / 300 = 1   = 100.00%
100 -> 100 / 300 = 1/3 =  33.00%
50  ->  50 / 300 = 1/6 =  16.67%
0   ->   0 / 300 = 0   =   0.00%
```

### ![](/wiki/shared/mode/taiko.png) osu!taiko

![Accuracy = 0.5(number of GOOD + number of GREAT) / (number of BAD + number of GOOD + number of GREAT)](img/accuracy_taiko.png)

Ở taiko, DCX được tính theo DCX đối với các note trong một beatmap chia cho tổng số note trong một beatmap. DCX các note được tính như sau: GREAT (良) được tính là 100%(), GOOD(可) là 50% và MISS/BAD (不可) là 0% và nó cũng sẽ mất combo. Drum rolls và spinners không bị ảnh hưởng gì tới DCX.

### ![](/wiki/shared/mode/catch.png) osu!catch

![Accuracy = (number of droplets + number of drops + number of fruits) / (number of missed droplets + number of missed drops + number of missed fruits + number of droplets + number of drops + number of fruits)](img/accuracy_catch.png)

[Work In Progress, Sang tạm bản tiếng anh để hiểu cơ chế](/wiki/Accuracy/en.md#osu!catch)

### ![](/wiki/shared/mode/mania.png) osu!mania

![Accuracy = (50 \* number of 50s + 100 \* number of 100s + 200 \* number of 200s + 300 \* number of 300s + 300 \* number of MAXs) / 300(number of 0s + number of 50s + number of 100s + number of 200s + number of 300s + number of MAXs)](img/accuracy_mania.png )

Ở mania thì tương tự như [osu!standard](#osu!standard).

## Đồ thị hiệu suất

![Performance graph](img/performance_graph.jpg )

Đồ thị hiệu suất là biểu đồ hiển thị hiệu suất của player (dựa vào life bar) trong quá trình chơi (thời gian). Thông tin chi tiết được hiển thị khi di chuột vào bảng performance như hình trên(chỉ tác dụng sau khi hoàn thành một map).

### Độ chính xác

Khi di chuột vào performance graph, thông số sẽ hiển thị *Error* và *Unstable Rate*.

Do cách mà 2 mod [DT](/wiki/DT) (Double Time) và [HT](/wiki/HT) (Half Time) được thực thi, chỉ số của *Error* và *Unstable Rate* sẽ cấp số nhân theo beatmap. Để lấy giá trị thực khi chơi mod DT, chia kết quả với 1.5. Tương tự, nhân kết quả với 1.33 khi chơi mod HT

#### Error

*Error* luôn hiển thị 2 giá trị để biểu diễn: số note bị hit sớm và số note bị hit muộn.

#### Unstable Rate

Chỉ số *Unstable Rate* thể hiển tính đồng nhất của thời gian của các số hit, chỉ số này càng thấp thì càng tốt(Các pro gamer thường có chỉ số này dưới 100). Hãy nhớ rằng *Unstable Rate* chỉ "cân đong đo đếm" tính nhấn quán chứ không phải độ chính xác