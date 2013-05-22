# Fix CoffeeScript error reporting

https://github.com/meteor/meteor/pull/1052, packaged for Meteorite.

Add this to your smart.json in the "packages" section:

```
{
  ...
  "packages": {
    "coffeescript": {
      "git": "git://github.com/awwx/meteor-fix-coffeescript-error-reporting.git"
    }
  }
}
```

This overrides Meteor's coffeescript package with this one, which has
the error reporting fix applied.

Using this override will no longer be necessary once the the fix is in
a Meteor release.
