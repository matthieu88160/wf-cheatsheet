//how methods are written in an interface

 * Here were are creating an interface, which we are going to use  across some classes we create.
 * Those classes will implement the UserInterface into them.
 * These concrete classes will have to implement (if their parent has not already done so, in which case the concrete class would inherit those methods) the public method getId(); && the public    method setRoles(array $roles) <-- has to be an array.
 * The motivation behind creating an interface is to define a common behavior for the classes that implement it. It creates a contract that guarentees the implementing classes will have the behaviour that is defined in the interface.

 * Now have fun!

```php
interface UserInterface{

 	public function getId();
	public function setRoles(array $roles);
	   
}
```
	