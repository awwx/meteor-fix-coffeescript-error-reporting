# Obsolete

This package is obsolete: Meteor's coffeescript package now has the fix included.


## Fix CoffeeScript error reporting

This fix is now in Meteor's "devel" branch.

https://github.com/meteor/meteor/pull/1052, packaged for Meteorite.

Overrides Meteor's coffeescript package with a version which has the
error reporting fix applied.

Using this override will no longer be necessary once the the fix is in
a Meteor release.


## Using Meteorite

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


## Using Meteor

Add the fixed version to the "packages" subdirectory of your
application directory.

```
$ cd ~/myapp
$ mkdir packages   (if it doesn't exist already)
$ git clone git://github.com/awwx/meteor-fix-coffeescript-error-reporting.git packages/coffeescript
```
