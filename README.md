#### _Chim-s-uiuctf-writeup_
# Buy_buy_buy
![Challenge Description](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture1.png)

Discord của giải có 1 room tên là **charl1e-chapl1n**

![Challenge Room](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture2.png)

Ở đây sẽ có 1 con bot quản lý đấu giá tên là **The Auction House**

![The Auction House](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture3.png)

Ta thấy có 3 món nó đang bán đó là 
* **Flag Common**
* **Flag Rare**
* **Flag Ultra Rare**

khi mua được cả 3 món đó ta sẽ redeem được flag

Gõ **/help** để hiện rule ở đây

![The Auction House's rules](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture4.png)

Balance mặc định của mỗi người là **10.000** nên nhiệm vụ bây giờ là phải kiếm được **11.010.000** để redeem flag

**Mindset:**
>Theo như rule của phòng đấu giá, các items thuộc **type: collectable** là các items đảm bảo được các tiêu chí 
>* **nhanh**
>* **gọn**
>* **lời**
>
>Thế nên ta sẽ vứt các items khác qua một bên và chỉ tập trung spam **/buy** và **/sell** những items **collectable**

**Cách làm**:
>**_/initiate_**

Để tham gia
>**_/buy ```item_type:collectable``` ``` item:Shiny Pokemon Card``` ```number_of_items:1```_**

Để mua 1 Shiny Pokemon Card với giá **10.000**
>
>**_/sell ```item_type:collectable``` ``` item:Shiny Pokemon Card```_**

Để bán Shiny Pokemon Card thu được **15.000**
=> Mỗi lần bán **Shiny Pokemon Card** ta lời được **5.000**

Tiếp tục spam **/buy** và **/sell** đến khi có đủ tiền mua 2, 3 rồi **100 Shiny Pokemon Card**.
Sau khi đạt đến **100 Shiny Pokemon Card**, ta chuyển sang món đáng mua kế tiếp là **_Clout_**
>
>**/buy ```item_type:collectable``` ``` item:Clout``` ```number_of_items:40```**
>**/sell ```item_type:collectable``` ``` item:Clout```**

Tiếp tục spam Clout cho đến khi đủ **12.000.000** 
Và ta mua được 3 phần của flag
>**/buy ```item_type:single``` ``` item:Flag Common``` ```number_of_items:1```**
>
>**/buy ```item_type:single``` ``` item:Flag Rare``` ```number_of_items:1```**
>
>**/buy ```item_type:single``` ``` item:Flag Ultra Rare``` ```number_of_items:1```**
>
>**/Redeem_flags**

![Flag](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture5.png)

Flag: **uiuctf{at_the_bang_of_the_gavel_only_one_can_win}**

# Doot Doot
![Challenge Description](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture6.png)

Bài cho một link youtube: [**Đây nè**](https://www.youtube.com/watch?v=zNXl9fqGX40)
Dẫn đến 1 video có dạng script của phim Star Wars chạy chạy :v 
>Ngồi coi hết **8 tiếng** clip thì flag hiện ra thôi

![Flag](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture7.png)

Đùa đấy :v
Bài này chắc là cần _may mắn_ :v
Mình **_tua ngược từ dưới lên_** + **_preview_** bằng thanh cuộn thì thấy luôn. Tốn đúng 2p

Flag: **uiuctf{doot_d0ot_do0t_arent_you_tired_of_the_int4rnet?}**

# Emote
![Challenge Description](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture8.png)

Đúng như tên bài

Vào discord của giải gõ **:emote:**
Nó là một custom emoji của room

![Emote emoji](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture9.png)

Download emoji này về

Cho vào **stegsolve LSB bit 7 red**, **blue** hay **green** đều được
>_Nhưng chỉ 1 channel thôi đừng chọn cả 3_

![Flag](https://github.com/khiemgamo/Chim-s-uiuctf-writeup/blob/main/Markdown_1.0.1/Picture10.png)

Flag: **uiuctf{staring_at_pixels_is_fun}**
