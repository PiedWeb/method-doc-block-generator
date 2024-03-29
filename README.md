<p align="center"><a href="https://dev.piedweb.com">
<img src="https://raw.githubusercontent.com/PiedWeb/piedweb-devoluix-theme/master/src/img/logo_title.png" width="200" height="200" alt="Open Source Package" />
</a></p>

# Method Doc Block Generator

[![Latest Version](https://img.shields.io/github/tag/PiedWeb/method-doc-block-generator.svg?style=flat&label=release)](https://github.com/PiedWeb/method-doc-block-generator/tags)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/PiedWeb/method-doc-block-generator/Tests?label=tests)](https://github.com/PiedWeb/PiedWeb/actions)
[![Quality Score](https://img.shields.io/scrutinizer/g/PiedWeb/PiedWeb.svg?style=flat)](https://scrutinizer-ci.com/g/PiedWeb/PiedWeb)
[![Code Coverage](https://codecov.io/gh/PiedWeb/PiedWeb/branch/main/graph/badge.svg)](https://codecov.io/gh/PiedWeb/PiedWeb/branch/main)
[![Type Coverage](https://shepherd.dev/github/PiedWeb/PiedWeb/coverage.svg)](https://shepherd.dev/github/PiedWeb/PiedWeb)
[![Total Downloads](https://img.shields.io/packagist/dt/piedweb/method-doc-block-generator.svg?style=flat)](https://packagist.org/packages/piedweb/method-doc-block-generator)


## Install

Via [Packagist](https://img.shields.io/packagist/dt/piedweb/method-doc-block-generator.svg?style=flat)

```bash
$ composer req piedweb/method-doc-block-generator
```

## Usage

### MethodDocBlockGenerator CLI

Example :
```php

include 'vendor/autoload.php';

use \PiedWeb\MethodDocBlockGenerator\MethodDocBlockGenerator;

$output = '<?php
/**
';
foreach ($extensionList as $className) {
    $output .= (new MethodDocBlockGenerator())->run($className);
}
$output .= ' */
class PlatesTemplate extends Template { }';

file_put_contents('src/Service/PlatesTemplate.php', $output);
```

## Contributing

Please see [contributing](https://dev.piedweb.com/contributing)

## Credits

- [PiedWeb](https://piedweb.com) ak [Robind4](https://twitter.com/Robind4)
- [All Contributors](https://github.com/PiedWeb/:package_skake/graphs/contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.

[![Latest Version](https://img.shields.io/github/tag/PiedWeb/PiedWeb.svg?style=flat&label=release)](https://github.com/PiedWeb/PiedWeb/tags)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/PiedWeb/PiedWeb/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/PiedWeb/PiedWeb/master.svg?style=flat)](https://travis-ci.org/PiedWeb/PiedWeb)
[![Quality Score](https://img.shields.io/scrutinizer/g/PiedWeb/PiedWeb.svg?style=flat)](https://scrutinizer-ci.com/g/PiedWeb/PiedWeb)
[![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/PiedWeb/PiedWeb.svg?style=flat)](https://scrutinizer-ci.com/g/PiedWeb/PiedWeb/code-structure)
[![Total Downloads](https://img.shields.io/packagist/dt/piedweb/method-doc-block-generator.svg?style=flat)](https://packagist.org/packages/piedweb/method-doc-block-generator)
