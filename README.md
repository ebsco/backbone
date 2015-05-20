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


## What is different in this fork of Backbone?
This fork of Backbone is currently the same as Backbone **1.1.2** (e.g. master = Backbone tagged at **1.1.2**), but with the following differences:

1. router/history support for hashes for sections on the same page.  This does *not* include the code to navigate to the sections.
2. Deep object comparison in Model.set has been replaced with simple === style comparison.
3. Copy of previous model attributes is no longer maintained.  Public methods that depended this functionality have been remove:
  - model.previous
  - model.previousAttributes

## Why diverge from main-line Backbone?

This fork has diverged from main-line Backbone due to performance issues experienced with using many instances of models and collections.  This is in part exacerbated by our use of Backbone models as view models for UI components that bind to change events of data models, which are also Backbone models.  All told, the performance of models and collection, especially Backbone.Model.set, needed to be vastly improved, which this fork does.

## Original Backbone docs

Backbone supplies structure to JavaScript-heavy applications by providing models key-value binding and custom events, collections with a rich API of enumerable functions, views with declarative event handling, and connects it all to your existing application over a RESTful JSON interface.

For Docs, License, Tests, pre-packed downloads, and everything else, really, see:
http://Backbonejs.org

To suggest a feature, report a bug, or general discussion:
http://github.com/jashkenas/Backbone/issues

Backbone is an open-sourced component of DocumentCloud:
https://github.com/documentcloud

Many thanks to our contributors:
http://github.com/jashkenas/Backbone/contributors

Special thanks to Robert Kieffer for the original philosophy behind Backbone.
http://github.com/broofa
