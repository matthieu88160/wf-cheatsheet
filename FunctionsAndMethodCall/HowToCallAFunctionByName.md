In the case of we have a function name as string, it's possible to call it by using
this string.

```php
function myFunction(){}

$functionName = 'myFunction';
$functionName();
```

It could be useful in the case of call iteration.
If wa have to call three functions one after the others :

```php
$functions = [
	'myFunction1',
	'myFunction2',
	'myFunction3',
	'myFunction4',
	'myFunction5',
];

foreach($functions as $function) {
	// at 1 iteration $function is equal to myFunction1, so we call myFunction1
	// at 2 iteration $function is equal to myFunction2, so we call myFunction2
	// at 3 iteration $function is equal to myFunction3, so we call myFunction3
	// at 4 iteration $function is equal to myFunction4, so we call myFunction4
	// at 5 iteration $function is equal to myFunction5, so we call myFunction5
	$function();
}
```

This could be coded like this :

```php
for ($i = 1;$i <= 5;$i++) {
	$functionName = 'myFunction' . $i;
	// at first iteration, $functionName is equal to myFunction1
	// at second iteration, $functionName is equal to myFunction2
	// etc...
	$functionName();
}
```
