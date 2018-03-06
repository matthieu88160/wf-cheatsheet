
To iterate over normal array :

```php
foreach($array as $eachElements) {
	echo $eachElement;
}

for($i = 0;$i < count($array);$i++) {
	echo $array[$i];
}
```

To iterate over associative :

```php
foreach($array as $eachKey => $eachValues) {
	echo $eachValues . ' Located into ' . $eachKey;
}

for($i = 0;$i < count($array);$i++) {
	$key = array_keys($array)[$i];
	$value = array[$key];
	echo $value . ' Located into ' . $key;
}
```







