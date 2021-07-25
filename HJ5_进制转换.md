描述
写出一个程序，接受一个十六进制的数，输出该数值的十进制表示。

输入描述：
输入一个十六进制的数值字符串。注意：一个用例会同时有多组输入数据，请参考帖子https://www.nowcoder.com/discuss/276处理多组输入的问题。

输出描述：
输出该数值的十进制字符串。不同组的测试用例用\n隔开。

示例1
输入：
0xA
0xAA
输出：
10
170

```python
# coding=utf8
while 1:
    try:
        print(int(input(), 16))
    except Exception as e:
        break
```

```php
<?php

while($str=trim(fgets(STDIN))){
    echo hexdec($str),PHP_EOL;
}
```
