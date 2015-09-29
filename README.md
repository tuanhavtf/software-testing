

1. Group 57 :
----------------------------

- Trịnh Văn Tú
 
- Hà Anh Tuấn

2. Kết quả bài làm:
-------------
>   Bài toán Coupon Collector

#### a. Mã chương trình
```js
function couponCollector(number) {
    var collected = [];

    for(var i=0; i < number; i++) {
        collected[i] = false;
    }

    var iteration = 0, unique = 0;
    var random;
    while(unique < number) {
        random = Math.floor(number * Math.random());
        if(!collected[random]) {
            unique++;
            collected[random] = true;
        }
        iteration++;
    }
    return iteration;
}

```

### b. Đồ thị


3.Sử dụng esgraph để tạo đồ thị chương trình cho ngôn ngữ Javascript
-----------------------------------------------------------------

https://github.com/Swatinem/esgraph

### Cách sử dụng:

-   Cài đặt Nodejs để sử dụng công cụ npm

-   Cài đặt esgraph bằng cách sử dụng gói quản lý package npm của Nodejs: `npm install esgrath`

-   Chạy chương trình : `$ cat $file | esgraph | dot -Tpng > output.png`
