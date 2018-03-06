The below function receives an argument to set the property of firstname to the given argument and retuns the current object
The keyword this is used to refer to the current object and because it is an object and in PHP the way to access a property of an object is to use ->
	
The general term used for this kind of method (a method that sets a property) is a setter method

```php
    public function setFirstname($firstname)
    {
        $this->firstname = $firstname;
        return $this;		    
		
	}
```
	
This is a getter method, and its job is to return a property the firstname in this case, it doesnt receive any arguments because it simply returns a property. It is good practise to name your getter and setter methods to reference the property it you want to access
	
```php
	public function getFirstname()
    {
        return $this->firstname;
    }	
```


We are returning this from setter to be fluent. A fluent method allow to chain method calls like :

```php
	$user = new User();
	$user->addElement($something1)
		->addElement($something2)
		->addElement($something3)
		->addElement($something4);
```
