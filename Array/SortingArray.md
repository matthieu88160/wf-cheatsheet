How to sort array :

## Natural sort

```php
$myArray = [2, 6, 1, 4];
sort($myArray);
// $myArray become [1, 2, 4, 6]

$myArray = ['a'=>2, 'b'=>6, 'c'=>1, 'd'=>4];
sort($myArray);
// $myArray become [1, 2, 4, 6]
```

## Shuffle an array

```php
$myArray = [2, 6, 1, 4];
shuffle($myArray);
```

## Sort array by key

```php
$myArray = ['b'=>2, 'c'=>6, 'a'=>1, 'd'=>4];
ksort($myArray);
// $myArray become ['a'=>1, 'b'=>2, 'c'=>6, 'd'=>4]
```

## Define your own function

```php
$myArray = array('a' => 4, 'b' => 8, 'c' => -1, 'd' => -9, 'e' => 2, 'f' => 5, 'g' => 3, 'h' => -4);
uasort($myArray, function($a, $b) {
    if ($a == $b) {
        return 0;
    }
    return ($a < $b) ? -1 : 1;
});
// $myArray become ['a'=>1, 'b'=>2, 'c'=>6, 'd'=>4]
```

