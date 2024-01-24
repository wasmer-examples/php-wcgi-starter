This is a simple [PHP](https://php.org/) application template running using WCGI

## Getting Started

Modify the logic of your the PHP application in the `app/index.php` file.

```console
$ echo '<?php print("Hello, World!"); ?>' > ./app/index.php
```

You can run things locally with:

```
$ php -S app/index.php
```

Or you can also use `wasmer run`:

```console
$ wasmer run . --net
```

> [!NOTE]
> You will need to have Wasmer installed (check out [the docs to install the Wasmer CLI](https://docs.wasmer.io/install)!). 
> The `--net` flag is required to enable networking support in Wasmer.

## Deploy on Wasmer Edge

The easiest way to deploy your PHP app is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: http://wcgi-php-starter-template.wasmer.app/

Run this commmand to deploy to Wasmer Edge:

```bash
wasmer deploy
```

> [!NOTE]
> You will need to change the namespace in `wasmer.toml` to your own namespace and app name in `app.yaml` to your own app name.
