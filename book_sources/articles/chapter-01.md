# 第一章

這是第一章的內容

編輯第一章 blarblar

## C
{%ace edit=true, lang='c_cpp'%}
// This is a hello world program for C.
#include <stdio.h>

int main(){
  printf("Hello World!");
  return 1;
}
{%endace%}

## JS Example
```eval-js
[1,2,3].map(function(x) { return x + 1;})
```

## PHP Example
```php
require dirname(__FILE__).'/source/class/class_core.php';
require dirname(__FILE__).'/source/class/class_load.php';
$load = new Load;
$load->loadDBClass('db_read');

//Main Logic
$result = array('url' => false);
if (isset($_GET['key']) && $_GET['key'] === IMAGE_KEY) {
    //Get image info
    $get_data = DataRead::getInstance();
    $get_data->getConnection($conn);
    $result = $get_data->getRandomImage();
    if ($result !== false && $result['album_id'] !== null) {
        if (file_exists($result['file_path'].'_s.'.$result['file_type'])) {
            $result['file_path'] = $base_url.'/'.$result['file_path'];
            $result['file_path'] .= '_s.'.$result['file_type'];
            $result = array('url' => $result['file_path'], 'album_id' => $result['album_id']);
        }
    }
}
exit(json_encode($result));
```
