Data can be inserted into array at creation :

```php
$myArray = ['some', 'value'];
```

To add some value to the array after the creation, we will have some syntax:

```php
$myArray[] = 'valueToAdd';

array_push($myArray, 'valueToAdd');
```

To add value to associated array :

```php
$myArray['where_i_want_to_add'] = 'TheValueToInject';
```
