https://viblo.asia/p/tu-tao-composer-package-cho-php-n7prv33ovKod

Cách sử dụng
Trên file composer.json của project muốn include package đó cần thêm vào dòng
   "require": {
        "kynm/hello-world": "dev-master"
    }
Dùng lệnh : composer update để load package về project
Trên file index của project cần require file autoload
require_once __DIR__ . '/vendor/autoload.php';
Khi sử dụng chỉ cần sử dụng đúng namespace:
use kynm\SayHello\Sayhello;
$hello = new SayHello();
echo $hello->world();
