### PHP is a single Inheritance language
You can not extends class from more than one class
### Traits
### [Overloading](https://www.php.net/manual/en/language.oop5.overloading.php)
Overloading in PHP provides means to dynamically create properties and methods. 
* Property overloading
```php
  public __set(string $name, mixed $value): void
```
```php 
  public __get(string $name): mixed
```
```php 
  public __isset(string $name): bool
```
```php
  public __unset(string $name): void
```
* Method overloading
```php
  public __call(string $name, array $arguments): mixed
```
```php 
  public static __callStatic(string $name, array $arguments): mixed
```
### Magic Methods
Magic methods are special methods which override PHP's default's action when certain actions are performed on an object.
The following method names are considered magical: 
* `__construct()`
* `__destruct()`
* `__call()`
* `__callStatic()`
* `__get()`
* `__set()`
* `__isset()`
* `__unset()`
* `__sleep()`
* `__wakeup()`
* `__serialize()`
* `__unserialize()`
* `__toString()`
* `__invoke()`
* `__set_state()`
* `__clone()`
* and `__debugInfo()`
### [Late static bindings](https://www.php.net/manual/en/language.oop5.late-static-bindings.php)

### [Scope Resolution Operator (::)](https://www.php.net/manual/en/language.oop5.paamayim-nekudotayim.php)
### [Type Juggling](https://www.php.net/manual/en/language.types.type-juggling.php)
PHP may attempt to convert the type of a value to another automatically in certain contexts.
### [Type Casting](https://www.php.net/manual/en/language.types.type-juggling.php#language.types.typecasting)
Type casting converts the value to a chosen type by writing the type within parentheses before the value to convert.
```php
  $foo = 10;   // $foo is an integer
  $bar = (bool) $foo;   // $bar is a boolean
```
