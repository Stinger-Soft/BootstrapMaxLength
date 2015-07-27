# Bootstrap MaxLength Js Bundle for Symfony2
Bootstrap MaxLength Js Bundle for Symfony2

## Current Version

Bootstrap MaxLength Js v1.6.0

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/boostrap-maxlength-js-bundle": "~1.6"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\BootstrapMaxLengthJsBundle\StingerBootstrapMaxLengthJsBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/boostrap-maxlength-js-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

Add the css and js file where needed:

``` html
{% javascripts
	'bundles/stingerbootstrapmaxlengthjs/js/bootstrap-maxlength.min.js'
%}
	<script src="{{ asset_url }}" ></script>
{% endjavascripts %}
```


# Licenses

Refer to the source code of the included files for license information

# References

1. https://github.com/mimo84/bootstrap-maxlength/
2. http://symfony.com