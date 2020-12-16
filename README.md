![Captcha](https://ghaninia.ir/filemanager/uploads/photos/1/download.png)

Installation
------------

Enter the following command to install Captcha
```php
$ composer require ghaninia/captcha
```
Now you have to add the package to your project by entering the following command
```php
...config/app.php

'providers' => [
    ...
    GhaniniaIR\Captcha\CaptchaServiceProvider::class 
],
```

usage 
-----
<p>Use the following command at the top of each file of the use Verta class
</p>

```html
<img src="{{ route("captcha") }}">
```

Validation Rules
-----

<p>
You can validate form with Validator Laravel
</p>

```php
$this->validate([
    "field" => 'required|captcha'
])
```

