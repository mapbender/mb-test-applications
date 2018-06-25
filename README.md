# Test applications for Mapbender.

## Installation:

- Extract the applications to: \<mapbender-starter\>/application/app/config/applications
- Clear the cache (application/app/cache/dev and application/app/cache/prod directory)

## Usage:

To change an application and to see the results directly, open Mapbender in development-mode with the app_dev.php file (see: https://doc.mapbender.org/en/faq.html?highlight=app_dev#app-php-und-app-dev-php-what-purpose-do-they-have).


## Files

### ol4 directory

Test cases for the OpenLayer 4 tests. They should still work with OL2 but if an element gets a new parameter or looses one, they might be only valid for OL4.

Most of the applications are built up the same: Map, Navigation Toolbar, buton-bar, footer and layertree in the sidebar. Most of them use the same services, like OSM and perhaps an internal one (where you might not have access to).

The "naked" variants only contain the needed elements, like the map (of course) and the element itself. These tests are for testing without side-effects.
