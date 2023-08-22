**PHP Basic Concept**
- CLASS
    - It is called magic property and its return current class name
```php
    __CLASS__
```

- __get($property)
    - It is called magic method. It is used to return specific property.
```php
    class Test
    {
        private $name = 'test';

        public function __get($property)
        {
            if(property_exists($this,$property))
            {
                return $this->$property;
            }
        }
    }
```
- __set($property, $value)
    - It is called magic method. It is used to set specific property value.

```php
    class Test
    {
        private $name = 'test';

        public function __set($property,$value)
        {
            if(property_exists($this,$property))
            {
                $this->$property = $value;
            }
        }
    }
```

**Create Folder Structure**
- app
    - config
    - controllers
    - helpers
    - models
    - views
    

