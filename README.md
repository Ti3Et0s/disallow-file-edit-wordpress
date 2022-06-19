# disallow-file-edit-wordpress

## In wp-config.php
```
define('DISALLOW_FILE_EDIT', true);

define('DISALLOW_FILE_MODS', true);
```
# OR

## In Functions.php

```
function disable_mytheme_action() {

  define('DISALLOW_FILE_EDIT', true);

  define('DISALLOW_FILE_MODS', true);

}
add_action('init','disable_mytheme_action');
```
