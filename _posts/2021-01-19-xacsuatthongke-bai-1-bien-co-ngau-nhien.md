---
layout: post
title: Xác suất thống kê-Biến cố ngẫu nhiên.
date: 2021-01-19 15:22:15 +0700
summary: Mô tả các khái niệm tổng quát và ôn tập tổ hợp.
categories: math
---

# Giới thiệu

## Mục đích của nghiên cứu lý thuyết xác suất
Nghiên cứu các hiện tượng ngẫu nhiên xảy ra trong cùng một điều kiện xác định cho kết quả khác nhau, ngược lại là hiện tượng tất định xảy ra trong cùng một điều kiện xác định cho kết quả giống nhau. Nói một cách đơn giản, mục đích nghiên cứu các hiện tượng ngẫu nhiên trong cùng một điều kiện thì lại cho ra các kết quả khác nhau.

Ví dụ: một viên xúc xắc đồng chất được gieo đúng ba lần ở cùng một vị trí. Nhưng kết quả của ba lần gieo là khác nhau.

## Lược sử
Xác suất bắt nguồn từ các trò chơi đỏ đen may rủi, các nhà toán học bắt đầu nghiên cứu về xác suất. Tuy nhiên, thời điểm đó, xác suất vẫn chưa phải là một môn khoa học. Mãi cho đến khi nhà toán học người Nga Andrey Nikolaevich Kolmogorov áp dụng lý thuyết tổ hợp và vi tích phân thì xác suất mới trở thành môn khoa học để nghiên cứu.

# Phép thử và biến cố
Khi quan sát một hiện tượng có xảy ra hay không? Ta quan sát xảy ra nhiều lần, và mỗi lần được gọi là phép thử ($$ \tau $$). 

Việc có xảy ra hay không trong kết quả của một phép thử được gọi là “biến cố ngẫu nhiên”.

Tập hợp tất cả các khả năng có thể xảy ra được gọi là không gian mẫu (outcome) $$ \Omega $$. Giả sử, khi tung xúc xắc, tất cả các trường hợp xảy ra là 1, 2, 3, 4, 5, 6. Vậy không gian mẫu là:
$$ \Omega = \left \{ 1, 2, 3, 4, 5, 6 \right \} $$ .

Các phần tử của không gian mẫu được gọi là biến cố sơ cấp (elementary event) $$ \omega $$. Giả sử, khi tung xúc xắc, biến cố sơ cấp là 1, hoặc biến cố sơ cấp là 2,…

Tập con của không gian mẫu là biến cố $$ A $$ (event) hay là biến cố ngẫu nhiên. Lấy ví dụ ở trên, khi tung xúc xắc, môt biến cố là $$ \left \{ 1, 2 \right \},\left \{ 6, 2, 5 \right \},... $$

# Loại biến cố
Một tập hợp $$ \Omega $$ sẽ có ít nhất có hai tập hợp con bao gồm $$ \varnothing $$ và tập chính nó $$ \Omega $$.

Biến cố là tập hợp con của không gian mẫu. Vì thế, một biến cố sẽ có chắc chắn hai loại biến cố:
+ Biến cố chắc chắn: kí hiệu là $$ \Omega $$, đây là biến cố nhất định xảy ra. Ví dụ, biến cố xuất hiện khi gieo xúc xắc nhỏ hơn 7. Đây là điều chắc chắn, vì bạn chỉ có thể gieo ra số nút từ 1 đến 6.
+ Biến cố không thể: kí hiệu là $$ \varnothing $$, đây là biến cố nhất định không xảy ra. Ví dụ, biến cố xuất hiện khi gieo xúc xắc bằng 7. Vì không bạn không thể gieo xúc xắc ra kết quả là 7 nút được. Hoặc biến cố tung đồng xu sao cho mặt sấp và mặt ngửa cùng xuất hiện, đây là điều không thể.

# Mối liên hệ giữa các biến cố

## Sự kéo theo
A kéo theo B, tức là A là con của B, kí hiệu $$ A \subset B $$, nếu A xảy ra thì B xảy ra, nhưng B xảy ra chưa chắc A xảy ra.
Ví dụ: Khi tung xúc xắc, Biến cố A là tập hợp tất cả các nút chia hết cho 4. Biến cố B là tập hợp tất cả các nút chia hết cho 2. Vậy bạn có thể thấy các số chia hết cho 4 thì kéo theo các số đó cũng chia hết cho 2, nhưng các số chia hết cho 2 thì không chắc sẽ chia hết cho 4, như 6 chia hết cho 2 nhưng không chia hết cho 4.

## Sự tương đương
A tương đương với B, kí hiệu là $$ A = B $$, nếu A xảy ra thì B xảy ra và ngược lại.
Ví dụ: khi tung xúc xắc, biến cố A là tập hợp tất cả các nút bằng 1. Biến cố B là tập hợp tất cả các nút nhỏ hơn 2. Vậy bạn chỉ có thể gieo ra 1 nút mới thoả.

## Biến cố tổng
Là tổng của A và B, kí hiệu A + B hoặc $$ A \cup  B $$ hay còn gọi là hợp. Là biến cố xảy ra nếu có ít nhất một trong hai biến cố xảy ra.

## Biến cố tích
Là tích của A và B, kí hiệu AB hoặc $$ A \cap B $$ hay còn gọi là giao. Là biến cố xảy ra nếu A và B đồng thời xảy ra. 

## Biến cố đối lập
là biến cố mà biến cố $$A$$ đang xét sẽ không xảy ra, kí hiệu $$ \bar{A}$$ 

## Biến cố hiệu 
Biến cố hiệu của A và B là biến cố A xảy ra nhưng biến cố B không xảy ra, kí hiệu $$A \setminus B$$. Ta có công thức hay sử dụng: $$ A \setminus B = A.\bar{B} $$.

## Biến cố xung khắc
Là biến cố khi A và B nếu xung khắc nhau, thì A không bao giờ xảy ra đồng thời với B. Định nghĩa toán học: $$ A\cap B = A.B = \varnothing $$. Hay nói một cách dễ hiểu là không bao giờ xảy ra.
Ví dụ: gọi A là biến cố của "các số chia hết cho 2 và lớn hơn 1 nhỏ hơn 7", gọi B là biến cố của "các số không chia hết cho 2 lớn hơn 2 và nhỏ hơn 6".
Vậy $$ A = \left \{ 2, 4, 6  \right \} $$ và $$ B = \left \{ 3, 5 \right \} $$
