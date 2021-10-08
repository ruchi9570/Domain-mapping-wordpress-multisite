# Domain-mapping-wordpress-multisite
A WordPress Multisite doamin mapping plugin 

Installation - 

We recommend dropping Mercator's directory into your mu-plugins directory. You may need to rename the folder from Mercator-master to mercator.

Then create a wp-content/sunrise.php file with the following:


// Default mu-plugins directory if you haven't set it
defined( 'WPMU_PLUGIN_DIR' ) or define( 'WPMU_PLUGIN_DIR', WP_CONTENT_DIR . '/mu-plugins' );

require WPMU_PLUGIN_DIR . '/mercator/mercator.php';

Additionally, in order for sunrise.php to be loaded, you must add the following to your wp-config.php:

define('SUNRISE', true);

Aliases are created in the Network Admin > Sites > Edit Site screen.
