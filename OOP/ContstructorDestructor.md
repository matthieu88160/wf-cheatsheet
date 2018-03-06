//What are a constructor and destructor

* A constructor is a function in a class that may be used to set its properties so that when we instantiate this class to create an object those properties get initialized. These properties can be set/initialized both with the use of a parameter or without.

* A destructor is also a function in class that's use in order to unset the properties of an object once the runtime is completed/finished.

```php

class Student {
  private $firstName;
  protected $lastName;

  public function __construct($firstName = "Ivan", $lastName = "Mendoza"){
    $this->firstName = $firstName;
    $this->lastName = $lastName;
  }
}

$ivan = new Student();
$sam = new Student("Sam", "Courtois");

```
