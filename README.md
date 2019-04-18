# MonsterID

[![Packagist](https://img.shields.io/packagist/v/sandfoxme/monsterid.svg)](https://packagist.org/packages/sandfoxme/monsterid)
[![license](https://img.shields.io/github/license/sandfoxme/monsterid.svg)](https://opensource.org/licenses/MIT)
[![Travis](https://img.shields.io/travis/sandfoxme/monsterid.svg)](https://travis-ci.org/sandfoxme/monsterid)
[![Code Climate Coverage](https://img.shields.io/codeclimate/c/sandfoxme/monsterid.svg)](https://codeclimate.com/github/sandfoxme/monsterid/coverage)
[![Code Climate](https://img.shields.io/codeclimate/maintainability/sandfoxme/monsterid.svg)](https://codeclimate.com/github/sandfoxme/monsterid)

MonsterID is a method to generate a unique monster image based upon a certain identifier
(IP address, email address, whatever).
It can be used to automatically provide personal avatar images in blog comments or other community services.

![Monster Example](docs/images/example.png)

MonsterID was inspired by a post by [Don Park] and the [Combinatoric Critters].

All graphics were created by [Andreas Gohr].
The source code and the graphics are provided under the [MIT License].

## Installation

Install it with Composer

``composer require 'sandfoxme/monsterid:^1.2'``.

## Usage

```php
<?php

use function \SandFox\MonsterID\build_monster;

header('Content-type: image/png');
echo build_monster('sandfox@sandfox.me', 150);
```

Read full documentation here: <https://sandfox.dev/monsterid.html>

## Adaptation

Adaptation as a composer library performed by [Anton "Sand Fox" Smirnov][SandFox]

[Don Park]:               http://www.docuverse.com/blog/donpark/2007/01/18/visual-security-9-block-ip-identification
[Combinatoric Critters]:  http://www.levitated.net/bones/walkingFaces/index.html
[Andreas Gohr]:           http://www.splitbrain.org
[MIT License]:            https://opensource.org/licenses/MIT
[SandFox]:                https://sandfox.me/
