This is a simple [PHP](https://php.org/) application template running using WCGI

## Getting Started

Modify the logic of your the PHP application in the `app/index.php` file.

```console
$ echo '<?php print("Hello, World!"); ?>' > ./app/index.php
```

You can run things locally with:

```
$ php -t app -S localhost:8080
```

Or you can also use `wasmer run` to run it locally (check out the [Wasmer install guide](https://docs.wasmer.io/install)):

```console
$ wasmer run . --net
```


> [!TIP]
> You can also run `wasmer run wasmer-examples/php-wcgi-starter --net`to run the remote package


## Deploy on Wasmer Edge

The easiest way to deploy your PHP app is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://wcgi-php-starter-template.wasmer.app/

Run this commmand to deploy to Wasmer Edge:

```bash
wasmer deploy
```

> [!NOTE]
> You will need to change the namespace in `wasmer.toml` to your own namespace and app name in `app.yaml` to your own app name.
