描述
输入一个int型整数，按照从右向左的阅读顺序，返回一个不含重复数字的新的整数。
保证输入的整数最后一位不是0。
输入描述：
输入一个int型整数

输出描述：
按照从右向左的阅读顺序，返回一个不含重复数字的新的整数

示例1
输入：
9876673
输出：
37689


```python
# coding=utf8

s = input()[::-1]
temp = ''
for i in s:
    if i not in temp:
        temp += i
print(temp)
```

```php
<?php
$arr = array_map('intval', str_split(strrev(trim(fgets(STDIN)))));
echo implode(array_unique($arr));
```
