描述
功能:输入一个正整数，按照从小到大的顺序输出它的所有质因子（重复的也要列举）（如180的质因子为2 2 3 3 5 ）

最后一个数后面也要有空格

输入描述：
输入一个long型整数

输出描述：
按照从小到大的顺序输出它的所有质数的因子，以空格隔开。最后一个数后面也要有空格。

示例1
输入：180
输出：2 2 3 3 5


```python
# coding=utf8

n = int(input())
for i in range(2, int(n**0.5+2)):
    while(n % i == 0):
        print(i, end=' ')
        n = int(n/i)
if n > 1:
    print(n, ' ')
```

```php
<?php

$n = (int)fgets(STDIN);
for($i=2; $i<=$n/$i; $i++){
    while($n%$i==0){
        echo $i,' ';
        $n /=$i;
    }
}
if($n > 1){
    echo $n, ' ';
}
```
