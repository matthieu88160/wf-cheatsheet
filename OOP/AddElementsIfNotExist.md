how to update an array with new values (needle and haystack)

args: 

 * $role; Role object, coming from OUTSIDE the object
 * $roles; is an array, is a variable INSIDE THIS object

```php
public function addRole(Role $role)
{
	if (!in_array($role, $this->roles)) { //if NOT in array
		array_push($this->roles, $role); //add the role at the END of the array
		// $this->roles[] = $role;
	}

	return $this;
}	
```