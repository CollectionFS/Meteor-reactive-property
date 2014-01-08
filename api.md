#ReactiveProperty
A simple class that provides an reactive property interface

#### <a name="ReactiveProperty"></a>new ReactiveProperty(defaultValue)&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-

__Arguments__

* __defaultValue__ *{any}*  
Set the default value for the reactive property

-
This api should only be in the internal.api.md

> ```ReactiveProperty = function(defaultValue) { ...``` [reactive-property.js:10](reactive-property.js#L10)

-

#### <a name="ReactiveProperty.get"></a>*reactiveproperty*.get()&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-
*This method __get__ is defined in `ReactiveProperty`*
Usage:
```js
  var foo = new ReactiveProperty('bar');
  foo.get(); // equals "bar"
```

> ```self.get = function() { ...``` [reactive-property.js:36](reactive-property.js#L36)

-

#### <a name="ReactiveProperty.set"></a>*reactiveproperty*.set(value)&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-
*This method __set__ is defined in `ReactiveProperty`*

__Arguments__

* __value__ *{any}*  

-
Usage:
```js
  var foo = new ReactiveProperty('bar');
  foo.set('bar');
```

> ```self.set = function(value) { ...``` [reactive-property.js:50](reactive-property.js#L50)

-

#### <a name="ReactiveProperty.dec"></a>*reactiveproperty*.dec([by])&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-
*This method __dec__ is defined in `ReactiveProperty`*

__Arguments__

* __by__ *{number}*    (Optional = 1)
Value to decrease by

-
Usage:
```js
  var foo = new ReactiveProperty('bar');
  foo.set(0);
  foo.dec(5); // -5
```

> ```self.dec = function(by) { ...``` [reactive-property.js:67](reactive-property.js#L67)

-

#### <a name="ReactiveProperty.inc"></a>*reactiveproperty*.inc([by])&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-
*This method __inc__ is defined in `ReactiveProperty`*

__Arguments__

* __by__ *{number}*    (Optional = 1)
Value to increase by

-
Usage:
```js
  var foo = new ReactiveProperty('bar');
  foo.set(0);
  foo.inc(5); // 5
```

> ```self.inc = function(by) { ...``` [reactive-property.js:82](reactive-property.js#L82)

-

#### <a name="ReactiveProperty.getset"></a>*reactiveproperty*.getset([value])&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ####
-
*This method __getset__ is defined in `ReactiveProperty`*

__Arguments__

* __value__ *{any}*    (Optional)
Value to set property - if undefined the act like `get`

-

__Returns__  *{any}*
Returns value if no arguments are passed to the function
Usage:
```js
  var foo = new ReactiveProperty('bar');
  foo.getset(5);
  foo.getset(); // returns 5
```

> ```self.getset = function(value) { ...``` [reactive-property.js:98](reactive-property.js#L98)

-
