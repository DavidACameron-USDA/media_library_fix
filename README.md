# Media Library Fix

A bug exists in Drupal Core when attempting to reference the Media Library to
reference a Media entity from an inline block in Layout Builder.  The Media
Library widget ultimately ends up checking for the Administer Blocks permission
which normally should not be required for that operation.  See
https://www.drupal.org/project/drupal/issues/3106315 for further details.

This module implements a work-around for the issue that was copied from this
comment: https://www.drupal.org/project/drupal/issues/3106315#comment-14068301.

