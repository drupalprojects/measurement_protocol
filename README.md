# Overview

This module provides some helper methods for sending data to [Google's Measurement Protocol][info] system. This is useful if you're tracking data within an API or in a way that doesn't give you access to traditional Google Analytics.

For more information on what data you can send, see [this reference][reference].

[info]: https://developers.google.com/analytics/devguides/collection/protocol/v1/
[reference]: https://developers.google.com/analytics/devguides/collection/protocol/v1/reference

# Usage

To use this module, you'll call one or more of the helper functions:

* `mptph()` - Tracks a page hit. 
* `mpte()` - Tracks a generic event.

## Example

To track a page hit: 

    // Will send a page hit to GAMP.
    mptph(array('title' => 'My page', 'page' => 'my-page');

The rest of the types are not implemented, but could be implemented very easily. Patches accepted.