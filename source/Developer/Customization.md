# Customization

For Configuration of the module please check the section Configuration in the user manual above.

Further customizations can be achieved through overloading of the source code. Use the existing implementations as reference.

## Options

The appearance and behavior of the TinyMCE editor can be adapted to individual preferences through various <a target="_blank" href="https://www.tiny.cloud/docs/configure">Settings</a>. Each configuration is implemented as a separate class. These are located in the folder 'Application/Core/TinyMCE/Options' of the module.

### Add

- To add an option, create a new class that fulfills the interface 'O3\TinyMCE\Application\Core\TinyMCE\Options\OptionInterface'.
- In the class 'O3\TinyMCE\Application\Core\TinyMCE\Configuration' extend the method 'addCustomOptions' and execute the call '$this->addOption()' in it with the instance of your created class.

### Modify

To change the settings of an existing option, overload its class and modify the return value of the corresponding method.

### Remove

In the class 'O3\TinyMCE\Application\Core\TinyMCE\Configuration' extend the method 'addCustomOptions' and execute the call '$this->removeOption()' in it with the ID of the option to be removed.

## Plugins

The functions of the editor can be controlled by plugins. Each function is usually represented by a button in the editor. For functions not included in the standard, the path to JavaScript files describing their functionality can be defined.

### Add

- To add a plugin, create a new class that fulfills the interface 'O3\TinyMCE\Application\Core\TinyMCE\Plugins\PluginInterface'.
- In the class 'O3\TinyMCE\Application\Core\TinyMCE\Pluginlist' extend the method 'get' and add an additional entry to the return with the instance of your created class.

### Modify

To change the settings of an existing plugin, overload its class and modify the return value of the corresponding method.

### Remove

In the class 'O3\TinyMCE\Application\Core\TinyMCE\Pluginlist' extend the method 'get' and remove the entry to be deleted in the return value.

## Toolbars

The function buttons in the editor are grouped into thematic toolbars which can be arranged individually.

### Add

- To add a toolbar, create a new class that fulfills the interface 'O3\TinyMCE\Application\Core\TinyMCE\Toolbar\ToolbarInterface'. 
- In the class 'O3\TinyMCE\Application\Core\TinyMCE\ToolbarList' extend the method 'get' and add an additional entry to the return with the instance of your created class.

### Modify

To change the settings of an existing toolbar, overload its class and modify the return value of the corresponding method.

### Remove

In the class 'O3\TinyMCE\Application\Core\TinyMCE\ToolbarList' extend the method 'get' and remove the entry to be deleted in the return value.
