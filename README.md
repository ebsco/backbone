     ____                     __      __
    /\  _`\                  /\ \    /\ \                                   __
    \ \ \ \ \     __      ___\ \ \/'\\ \ \____    ___     ___      __      /\_\    ____
     \ \  _ <'  /'__`\   /'___\ \ , < \ \ '__`\  / __`\ /' _ `\  /'__`\    \/\ \  /',__\
      \ \ \ \ \/\ \ \.\_/\ \__/\ \ \\`\\ \ \ \ \/\ \ \ \/\ \/\ \/\  __/  __ \ \ \/\__, `\
       \ \____/\ \__/.\_\ \____\\ \_\ \_\ \_,__/\ \____/\ \_\ \_\ \____\/\_\_\ \ \/\____/
        \/___/  \/__/\/_/\/____/ \/_/\/_/\/___/  \/___/  \/_/\/_/\/____/\/_/\ \_\ \/___/
                                                                           \ \____/
                                                                            \/___/
    (_'_______________________________________________________________________________'_)
    (_.———————————————————————————————————————————————————————————————————————————————._)


## What is different in this fork of backbone?
This fork of backbone is currently the same as backbone **1.1.2** (e.g. master = backbone tagged at **1.1.2**), but with the following differences:

1. router/history support for hashes for sections on the same page.  This does *not* include the code to navigate to the sections.
2. Deep object comparison in Model.set has been replaced with simple === style comparison.
3. Copy of previous model attributes is no longer maintained.  Public methods that depended this functionality have been remove:
  - model.previous
  - model.previousAttributes



Backbone supplies structure to JavaScript-heavy applications by providing models key-value binding and custom events, collections with a rich API of enumerable functions, views with declarative event handling, and connects it all to your existing application over a RESTful JSON interface.

For Docs, License, Tests, pre-packed downloads, and everything else, really, see:
http://backbonejs.org

To suggest a feature, report a bug, or general discussion:
http://github.com/jashkenas/backbone/issues

Backbone is an open-sourced component of DocumentCloud:
https://github.com/documentcloud

Many thanks to our contributors:
http://github.com/jashkenas/backbone/contributors

Special thanks to Robert Kieffer for the original philosophy behind Backbone.
http://github.com/broofa
