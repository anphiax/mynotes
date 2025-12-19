---
title: "My note"
date: 2025-12-16
draft: false
---

Hãy xem cách mà Euler, từ 3 thế kỉ trước đã tính tổng các nghịch đảo bình phương này như thế nào.

Ý tưởng của Euler là sự bằng nhau trong biểu diễn tổng và tích của một hàm và sau đó tìm ra quan hệ khi cân bằng các hệ số.
Ông bắt đầu với khai triển Maclaurin của sin x.
$$\sin x = x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!} + \cdots =\sum_{n=0}^{\infty} \frac{(-1)^n}{(2n+1)!}x^{2n+1}$$
Ở đây, sin x được biểu diễn như là một đa thức với bậc vô hạn. Vì là đa thức, nên nó có thể được viết lại dưới dạng tích của các thừa số có nghiệm của nó.

Vì sin x có các nghiệm là 0, $\pm \pi$, $\pm 2\pi$, $\pm 3\pi$,... nên nó có thể được viết lại dưới dạng tích. Ta có thể viết lại một chút. A này là một hằng số, nhưng cuối cùng nó cũng phải bằng 1 giới hạn sin x/x khi x tiến đến 0 bằng 1. Và ta viết lại dưới dạng gọn hơn như sau.

$$\begin{aligned}
\sin x &= x\left(x^2-\pi^2 \right)\left(x^2-4\pi^2 \right)\left(x^2-9\pi^2 \right)\cdots\\
&=Ax \left(1-\frac{x^2}{\pi^2}\right) \left(1-\frac{x^2}{2^2\pi^2}\right)\left(1-\frac{x^2}{3^2\pi^2}\right)\cdots\\
&=x \left(1-\frac{x^2}{\pi^2}\right) \left(1-\frac{x^2}{2^2\pi^2}\right)\left(1-\frac{x^2}{3^2\pi^2}\right)\cdots \\
&=x\prod_{n=1}^\infty \left(1-\frac{x^2}{n^2\pi^2}\right) 
\end{aligned}
$$

Như vậy, sin x bây giờ có thể được biểu diễn theo hai cách
$$\sin x = x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!} + \cdots = x\left(1-\frac{x^2}{\pi^2}\right) \left(1-\frac{x^2}{2^2\pi^2}\right)\left(1-\frac{x^2}{3^2\pi^2}\right)\cdots$$
Cân bằng hệ số của x^3, ta được
$$-\frac{1}{3!}=-\frac{1}{\pi^2}-\frac{1}{2^2\pi^2}-\frac{1}{3^2\pi^2}-\frac{1}{4^2\pi^2} - \cdots$$
Và đây chính là kết quả ban đầu.
$$\frac{1}{1^2}+ \frac{1}{2^2} + \frac{1}{3^2} +\frac{1}{4^2}+ \cdots = \frac{\pi^2}{6}$$
Trong tác phẩm Introductio của Euler vào năm 1748, bằng cách cân bằng các hệ số khác, ông đã liệt kê kết quả cho mũ 4, mũ 6, mũ 8, vân vân, đến mũ 26.

Để thấy được sự phức tạp của bài toán đến mũ 26, chúng tôi đưa ra đây kết quả của nó.
$$\frac{1}{1^{26}}+ \frac{1}{2^{26}} + \frac{1}{3^{26}} +\frac{1}{4^{26}}+ \cdots = \frac{1\;315\;862}{11\;094\;481\;976\;030\;578\;125}\pi^{26}$$
Nhớ rằng, Euler làm tất cả những điều này mà không cần một máy tính nào.

Phương pháp tính tổng tài tình của Euler đã trở thành ý tưởng cho Riemann, người mà sau ông hơn 100 năm, đã đưa ra giả thuyết Riemann nổi tiếng.




