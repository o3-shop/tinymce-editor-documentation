# Update

Open a terminal window and navigate to the main store directory.

Deactivate the module executing the command:

```
vendor/bin/oe-console oe:module:deactivate o3-tinymce-editor
```

Alternatively you can deactivate the module in the Shop Admin at 'Extensions' -> 'Modules'. Select the module and deactivate it in the tab 'Overview'.

```{note}
Every time the module is activated or deactivated the module does empty the files in the shop's tmp directory.'
```

The actual update is done executing the Composer command:

```
composer require o3-shop/tinymce-editor:^1.0
```

```{note}
Dependent on your server configuration you have to adjust the composer command. Please check your hosting support for details.
```

```{note}
The update will overwrite any changes you may have made to the module in the source directory.

Background: During an update, Composer first loads the new data into the **vendor** directory. Then the data is copied to the **source** directory. This replaces the files.
```

```{attention}
During the update you will be asked which packages may be overwritten.

Confirm the "o3-shop/tinymce-editor" query with *Yes*.
```

Activate the module executing the command:

```
vendor/bin/oe-console oe:module:activate o3-tinymce-editor
```

Alternatively you can activate the module in the Shop Admin at 'Extensions' -> 'Modules'. Select the module and activate it in the tab 'Overview'.
