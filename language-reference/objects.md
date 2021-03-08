# Objects

- Object has a method `__exit__()` that is run when closing the object. Similar to desctructor.
- Class items called attributes.
- Creation of object is made by calling class with ().
- First argument of any method — class instance, self.
- All atributes are public.
- If Python finds no attribute on instance, it will lookup on class.
- @staticmethod — works wih _class_ atributes and available for all instances; does not require self to be first attribute.
- When you set this decorator, you can call decorated method from any instance.
- @classmethod used for fabrics and method overload. Class methods a like regular methods, but relate to class as to object. Convention to use first argument `cls`.
- Method `__repr__(self)` returns string representation of the object.
- Method `__str__(self)` ?
