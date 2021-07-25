描述
输入一个int型的正整数，计算出该int型数据在内存中存储时1的个数。

输入描述：
 输入一个整数（int类型）

输出描述：
 这个数转换成2进制后，输出1的个数

示例1
输入：5
输出：2

```python
# coding=utf8
print(bin(int(input())).count('1'))
```

```php
<?php
echo substr_count(decbin(intval(fgets(STDIN))), '1');
```
