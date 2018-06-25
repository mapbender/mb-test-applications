# Test applications for Mapbender.

## Installation:

- Extract the applications to: \<mapbender-starter\>/application/app/config/applications
- Clear the cache (application/app/cache/dev and application/app/cache/prod directory)

## Usage:

To change an application and to see the results directly, open Mapbender in development-mode with the app_dev.php file (see: https://doc.mapbender.org/en/faq.html?highlight=app_dev#app-php-und-app-dev-php-what-purpose-do-they-have).


## Files

about_footer.yml: Simple application that provides an "About" button in the footer. The button opens a popup with a plain Mapbender version number.
about.yml: Simple application that provides an "About" button in the toolbar. The button opens a popup with a plain Mapbender version number.

activityindicator.yml: Simple application that provides the ActivityIndicator in the footer.
activityindicator_naked.yml: Simple application that provides the ActivityIndicator in the footer. It hides behind the Symfony-Toolbar if you are in developer mode.

arearuler_immediate_false.yml: AreaRuler application with button in toolbar. It does not calculate the drawn area immediately.
arearuler_immediate_true.yml: AreaRuler application with button in toolbar. It does calculate the drawn area immediately.
arearuler_naked.yml: Pure AreaRuler with button in toolbar and additional options commented out in .yml (for testing).
arearuler.yml: Default AreaRuler application with button in toolbar.

copyright_naked.yml: Pure Copyright application with additional options commented out in .yml (for testing).
copyright.yml: Default Copyright application which auto-opens the copyright popup and shows some fancy HTML.

digitizer_all_features.yml: Digitizer application which includes almost all documented digitizer options (https://doc.mapbender3.org/de/functions/editing/digitizer.html). Search for desired option in .yml for easy access. Clustering is commented out as it is an experimental feature. Events are not included.
digitizer.yml: Default digitizer configuration as published in Mapbender Documentation.

gpsposition_naked.yml: Pure GPSPosition application. Provides the GPS-Element with a button in the toolbar. Default configuration of options.
gpsposition.yml: Default GPSPosition application. Automatically zooms to your location if you open it.

imageexport_naked.yml: Pure ImageExport application.
imageexport.yml: Default ImageExport application that captures .png or .jpg files of the map.

layertree_dialog.yml
layertree_wo_groups_naked.yml:

legend_naked: Pure legend application.
legend_sidepane: Application with a legend embedded in the sidepane. All options are set "true".
legend.yml: Default legend application.

lineruler_immediate_false_yml: LineRuler application with button in toolbar. It does not calculate the drawn line length immediately.
lineruler_immediate_true.yml: LineRuler application with button in toolbar. It does calculate the drawn line length immediately.
lineruler_naked.yml: Pure LineRuler with button in toolbar and additional options commented out in .yml (for testing).
lineruler: Default LineRuler application with button in toolbar.

map_naked.yml: An application which features a map.

overview_naked.yml: Pure overview application which includes all configurational options.
overview.yml: Default application which features an overview map in the documented configuration.

print_naked.yml: Pure PrintClient integration with toolbar button, all options integrated (replace_pattern commented out)
print_sidepane.yml: PrintClient integrated in Sidepane, with additional feature to turn frame on/off (& replace_pattern commented out)
print.yml: Default PrintClient application with button in toolbar (& replace_pattern commented out).

redlining_dialog_naked.yml: Pure redlining application, includes a button in the toolbar that heads to the redlining_dialog.
redlining_imageexport.yml: Redlining and imageexport application to test the functionality between the elements.
redlining_print.yml: Redlining and print application to test the functionality between the elements.
redlining_sidepane_naked.yml: Pure redlining in the sidepane (application). Includes no other features.
redlining_sidepane.yml: Default redlining in the sidepane (application). Has the default tools.


### ol4 directory

Test cases for the OpenLayer 4 tests. They should still work with OL2 but if an element gets a new parameter or looses one, they might be only valid for OL4.

Most of the applications are built up the same: Map, Navigation Toolbar, button-bar, footer and layertree in the sidebar. Most of them use the same services, like OSM and perhaps an internal one (where you might not have access to). If not stated otherwise, you'll find these structures in the .yml-files above.

The "naked" variants only contain the needed elements, like the map (of course) and the element itself. These tests are for testing without side-effects.



### kombitest.json

An internal testcase.
