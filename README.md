# jsnlib-group

假設我們有這樣的陣列
````php 
$ary = array('a', 'b', 'c', 'd', 'e', 'f', 'g');
````

## 一、指定每個盒子最多有多少個
````php
$result = Jsnlib\Group::length($ary, 3);
print_r($result);

/*Array
(
    [0] => Array
        (
            [0] => a
            [1] => b
            [2] => c
        )

    [1] => Array
        (
            [0] => d
            [1] => e
            [2] => f
        )

    [2] => Array
        (
            [0] => g
        )

)*/
````

## 二、指定總共有多少個盒子
````php
$result = Jsnlib\Group::each($ary, 3);
print_r($result);

/*
Array
(
    [0] => Array
        (
            [0] => a
            [1] => d
            [2] => g
        )

    [1] => Array
        (
            [0] => b
            [1] => e
        )

    [2] => Array
        (
            [0] => c
            [1] => f
        )

)
 */
 ````
