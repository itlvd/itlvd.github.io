---
layout: post
title: Xác suất thống kê-Hoán vị Chỉnh hợp và Tổ hợp
date: 2021-01-20 15:22:15 +0700
summary: Giới thiệu về hoán vị, chỉnh hợp và tổ hợp. Cách tính nhanh chỉnh hợp và tổ hợp.
categories: math
---

# Hoán vị của n phần tử

Hoán vị n phần tử là một cách sắp xếp thứ tự n phần tử. Là số cách hoán đổi vị trí của n phần tử đó với nhau sao cho không trùng lặp.

__Ví dụ__: $$ \Omega = 1,2,3$$
Tổng số hoán vị là $$3! = 6$$. Bao gồm:
+ $$ \left \{ 1,2,3 \right \}$$.
+ $$ \left \{ 1,3,2 \right \} $$.
+ $$ \left \{ 2, 1, 3 \right \} $$.
+ $$ \left \{ 2,3,1 \right \}$$.
+ $$ \left \{ 3,1,2 \right \}$$.
+ $$ \left \{ 3,2,1 \right \}$$.

Hay giải theo cách mà mới học tổ hợp hay giải là:
+ Phần tử đầu tiên có $$3$$ cách chọn.
+ Phần tử thứ hai có $$2$$ cách chọn.
+ Phần tử thứ ba có $$1$$ cách chọn.
Vậy số hoán vị của $$3$$ phần tử là: $$3.2.1 = 6$$

__Ví dụ khác__: Có một bạn gái gửi cho mình bức thư tình, nhưng không muốn mình biết cô ấy là ai. Nên cô ấy cắt chữ: "anh, yêu, em, không" ở trong một tờ báo nào đó và kèm theo địa chỉ nơi gửi và nhận. Nhưng không may, trong quá trình gửi, các chữ cái bị xốc lên xốc xuống nên lộn xộn và mình nhận được thông điệp của cô gái là: "em, không, yêu, anh". Theo phản xạ của mình, mình sẽ gửi lại cho cô ấy thông điệp: "anh, không, yêu, em". Nhưng thế nào trên đường đi vấp ổ voi chữ nó lại lộn xộn và đến tay cô gái là: "không, anh, yêu, em". Mệt mỏi chưa, có 4 chữ, lộn qua lộn lại, yêu hay không yêu nói một lời. Tại thằng shipper đi không né ổ voi nên cuộc tình chúng ta ngang trái.

# Chỉnh hợp chập k của n phần tử

## Chỉnh hợp không lặp

Tương tự như hoán vị nhưng thay vì lấy hết $$n$$ phần tử, thì ta chỉ lấy $$k$$ phần tử. Tức là mỗi bộ sẽ có $$k$$ phần tử, các bộ đó có tính thứ tự và phải khác nhau.

<span class="red">Công thức:</span> $$ A_{n}^{k} = \frac{n!}{(n-k)!}$$

__Ví dụ__: Lớp học có 40 bạn học sinh. Mình cần chọn 3 bạn làm lớp trưởng, lớp phó học tập, lớp phó kỷ luật. Vậy số cách chọn 3 bạn trong 40 bạn là $$ A_{40}^{3} = \frac{40!}{(40-3)!} = 59280$$. Thế là mình gọi 3 bạn: "Dũng, Minh, Khôi". Thì:
+ <span class="green">Dũng</span> làm lớp trưởng, <span class="red">Minh</span> làm lớp phó học tập, <span class="yellow">Khôi</span> là lớp phó kỷ luật.
+ <span class="red">Minh</span> làm lớp trưởng, <span class="yellow">Khôi</span> làm lớp phó học tập, <span class="green">Dũng</span> làm lớp phó kỷ luật.
+ <span class="yellow">Khôi</span> làm lớp trưởng, <span class="red">Minh</span> làm lớp phó học tập, <span class="green">Dũng</span> làm lớp phó kỷ luật.
+ ...

> Cách xếp hoàn toán khác nhau, 3 bạn ấy chỉ cần thay đổi vị trí thì sẽ tạo ra một hoán vị mới.

Hay cách làm khi mới học tổ hợp:
+ Số cách chọn bạn thứ nhất làm lớp trưởng là: 40.
+ Số cách chọn bạn thứ hai làm lớp phó học tập là: 39 (vì 1 bạn làm lớp trưởng rồi).
+ Số cách chọn bạn thứ ba làm lớp phó kỷ luật là: 38 (1 bạn đã làm lớp trưởng, 1 bạn đã làm lớp phó học tập).

Nên số cách chọn 3 bạn trong 40 bạn đảm nhận 3 vị trí lớp trưởng, lớp phó học tập, lớp phó kỷ luật là: $$40.39.38 = 59280$$

## Giải thích công thức

 $$ A_{n}^{k} = \frac{n!}{(n-k)!}$$

__Ví dụ__ mình cần chọn 3 bạn trong 5 bạn học sinh. Thì $$ A_{5}^{3} = \frac{5!}{(5-3)!} = 60$$.

Cách làm khi mới học tổ hợp: $$5.4.3 = 60$$

Các bạn khai triển ra từ từ $$A_{5}^{3} = \frac{5!}{(5-3)!} = \frac{5.4.3.2.1}{2.1}=5.4.3 $$. Tới đây đã giống với cách phía trên. 

<span class="red">Giải thích</span>: Tức là bạn lấy hoán vị của 5 phần tử, bạn cần 3 phần tử nên bạn xem các phần tử phía sau là một (một ở đây tức là một phần tử, không phải các phần tử bằng một). Nên bạn chỉ cần chia số hoán vị của các phần tử phía sau là xong.

## Chỉnh hợp lặp

Chỉnh hợp lặp là chỉnh hợp và cho phép các phần tử được lặp lại.

$$n^{k}$$

__Ví dụ__:

Liệt kê các số có 4 chữ số từ tập $$ A = {1,2,3,4,5,6}$$.

+ Nếu tính chỉnh hợp không lặp $$A$$ là các ký tự khác nhau đôi một: 1234, 1245, 1245, 2635, 2413, ...

+ Nếu chỉnh hợp lặp $$B$$ là các ký tự có thể trùng nhau như: 1542, 1142, 1244, 1222, 5555, 5441, ...

=> $$A \subset B$$

__Thêm một ví dụ đơn giản__: 

Liệt kê các số có 2 chữ số trong tập : $$B = {0,1,2,3,4,5,6,7,8,9}$$

Giả sử, các bạn chưa biết tổ hợp thì số lượng các số có hai chữ số là từ $$00\rightarrow 99$$ là $$100$$ chữ số.

Số cách chọn chữ số đầu tiên là: $$10$$

Số cách chọn chữ số thứ hai là: $$10$$

Vậy số lượng các số có hai chữ số là: $$10^{2} = 100$$. Hay $$n^{k} = 10^{2} = 100$$.

# Tổ hợp chập k của n phần tử

Tương tự như chỉnh hợp. Nhưng khác một chỗ duy nhất là không cần vị trí. Vậy tổ hợp có hai tính chất: mỗi tổ hợp phải khác nhau, nhưng không tính thứ tự.

$$ C_{n}^{k} = \frac{n!}{k!.(n-k)!}$$

__Ví dụ__: Lớp học có 40 bạn học sinh. Mình cần chọn 3 bạn sau giờ học đi quét nhà. Vậy số cách chọn 3 bạn trong 40 bạn là $$ C_{40}^{3} = \frac{40!}{3!.(40-3)!} = 9880$$. Thế là mình gọi 3 bạn: "Dũng, Minh, Khôi". Thì:
+ <span class="green">Dũng</span> ở lại quét lớp, <span class="red">Minh</span> ở lại quét lớp, <span class="yellow">Khôi</span> ở lại quét lớp.
+ <span class="red">Minh</span> ở lại quét lớp, <span class="yellow">Khôi</span> ở lại quét lớp, <span class="green">Dũng</span> ở lại quét lớp.
+ <span class="yellow">Khôi</span> ở lại quét lớp, <span class="red">Minh</span> ở lại quét lớp, <span class="green">Dũng</span> ở lại quét lớp.
+ ...

> Với 3 cách trên thì nó là như nhau, nói bạn nào cũng như nhau. Vậy chỉ có 1 cách thôi.

<span class="red">Giải thích công thức</span>: $$ C_{n}^{k} = \frac{n!}{k!.(n-k)!}$$

Như đã nêu phía trên, tổ hợp là chỉnh hợp nhưng không tính vị trí. Nên nếu không tính vị trí thì...ta chia cho hoán vị của chúng là xong.

$$ C_{n}^{k} = \frac{n!}{k!.(n-k)!} = \frac{A_{n}^{k}}{k!}$$

# Cách tính nhẩm

Từ những công thức trên, nếu bạn hiểu được "Tại sao lại có công thức ấy" thì bạn sẽ tự nghĩ ra được cách tính nhẩm. Thực ra bạn hoàn toàn có thể bấm máy tính, chính xác hơn, nhưng các số nhỏ nhỏ thì tính tay nhanh hơn thời gian bạn bấm máy.

## Tính chỉnh hợp

Bạn có thể tính chỉnh hợp chập k của n. Nhưng với k nhỏ nhỏ thôi, cỡ $$k = 2$$ hoặc tối đa với mình là $$k=4$$.

Cách tính rất đơn giản: 
$$A_{5}^{3} = \frac{5!}{(5-3)!} = \frac{5.4.3.2.1}{2.1}=5.4.3$$
bạn có nhận ra với k bằng bao nhiêu thì ta lấy tích của các số từ n cho đến n - k. Để tránh hiểu sai, nên mình ghi hơi khó hiểu.

__Ví dụ__:

+ $$A_{5}^{3} = 5.4.3$$.
+ $$A_{15}^{4} = 15.14.13.12$$.
+ $$A_{10}^{2} = 10.9$$.

## Tính tổ hợp

Tương tự, sau khi tính chỉnh hợp xong thì chia cho $$k!$$. Đây là lý do mà mình nghĩ với các tổ hợp có $$k$$ nhỏ nhỏ thôi. Chia cho lẹ và khoẻ.
Mình nghĩ phép chia 1 đến 2 chữ số thì có lẽ đơn giản.

__Ví dụ__:

+ Với $$C_{5}^{3}$$, bạn tính $$A_{5}^{3}$$ trước, sau đó chia cho $$3! = 6$$.
+ Với $$C_{15}^{4} = 15.14.13.12$$, bạn tính $$A_{15}^{4}$$ trước, sau đó chia cho 4!.
+ ...

Nhìn có vẻ phép chia rối rắm, nhưng trong một số trường hợp bạn có thể tính nhanh và sử dụng khá ít phép tính.

__Ví dụ__:

+ Với $$C_{7}^{3}$$, bạn tính $$A_{7}^{3}$$ và chia cho $$3! = 6$$. Bạn có thể nhận xét:  $$A_{7}^{3} = 7.6.5$$ và $$3! = 6$$, ta được:

$$C_{7}^{3} = \frac{A_{7}^{3}}{3!} = \frac{7.6.5}{6} = 7.5 = 35$$

# Kết
Bài viết này, mình nêu các khái niệm về hoán vị, chỉnh hợp và tổ hợp. Và cách tính nhanh về hoán vị, chỉnh hợp, tổ hợp. Nếu có đóng góp ý kiến gì các bạn hãy để lại bình luận dưới bài viết nhé.
