描述
数据表记录包含表索引和数值（int范围的正整数），请对表索引相同的记录进行合并，即将相同索引的数值进行求和运算，输出按照key值升序进行输出。

输入描述：
先输入键值对的个数
然后输入成对的index和value值，以空格隔开

输出描述：
输出合并后的键值对（多行）

示例1
输入：
4
0 1
0 2
1 2
3 4
输出：
0 3
1 2
3 4

```python
# coding=utf8

n = int(input())
d = dict()
for _ in range(n):
    k, v = map(int, input().split())
    d[k] = d.get(k, 0) + int(v)

for key in sorted(d):
    print(key,d.get(key))
```

```php
<?php

$n = (int)fgets(STDIN);
$arr = [];
while($n){
  list($k, $v) = explode( ' ', fgets(STDIN));
  $k = (int)$k;
  $v = (int)$v;
  if(array_key_exists($k, $arr)){
      $arr[$k] +=$v;
  }else{
      $arr[$k] = $v;
  }
  $n--;
}
ksort($arr);
foreach($arr as $k=>$v){
    echo (int)$k, ' ', (int)$v,PHP_EOL;
}
```
