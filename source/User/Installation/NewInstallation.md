# New installation

```{note}
This module is part of the shop installation starting shop version 1.2.0. Hence following information is only relevant in case the module got removed.
```

Open a terminal window and navigate to the main store directory.

Install the module executing the Composer command:

```
composer require o3-shop/tinymce-editor:^1.0
```

```{note}
Dependent on your server configuration you have to adjust the composer command. Please check your hosting support for details.
```

Activate the module executing the command:

```
vendor/bin/oe-console oe:module:activate o3-tinymce-editor
```

Alternatively you can activate the module in the Shop Admin at *Extensions -> Modules*. Select the module and activate it in the tab *Overview*.

```{note}
Every time the module is activated or deactivated the module does empty the files in the shop's tmp directory.
```
