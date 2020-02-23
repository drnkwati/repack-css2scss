
css2less
========

This library aims to convert CSS files into SCSS files.

example
=======

The code below takes a few CSS instructions and prints them in a more SCSS like form:

```php
$cssContent = 'body p { font-family: arial; }';
$css2scssParser = new \Repack\Css2ScssPhp\Css2Scss($cssContent);
echo $css2scssParser->getScss();
```

output:

```
body {
        p {
                font-family: arial;
        }
}
```