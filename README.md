Installation
------------
before install package installed  <a href="http://image.intervention.io">intervention</a>

Copy Files and paste to root Directory
Open `Composer.json` files and go to `autoload >> psr-4`
append to object 
```bash
"GhaniniaIR\\Captcha\\" : "Package/GhaniniaIR/Captcha/src/"
```
open command line and enter 
```bash
composer dumpautoload
```
Add the service provider in config/app.php:
```php
GhaniniaIR\Captcha\CaptchaServiceProvider::class 
```
usage 
-----
```php
$this->validate([
    "field" => 'required|captcha'
])
```
```html
<img src="{{ route("captcha") }}">
```
