写出一个程序，接受一个由字母、数字和空格组成的字符串，和一个字母，然后输出输入字符串中该字母的出现次数。不区分大小写，字符串长度小于500。

输入描述：
第一行输入一个由字母和数字以及空格组成的字符串，第二行输入一个字母。

输出描述：
输出输入字符串中含有该字符的个数。

示例1
输入：
ABCabc
A
输出：2

```python
# coding=utf8

string = input().lower()
search = input().lower()
print(string.count(search))
```

```php
<?php
$str = strtolower(trim(fgets(STDIN)));
$search = strtolower(trim(fgets(STDIN)));
echo substr_count($str, $search);
```
