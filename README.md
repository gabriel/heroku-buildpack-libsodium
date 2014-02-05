# Heroku buildpack: libsodium

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for the `libsodium` library. It is used by the cryptography library [RbNaCl](https://github.com/cryptosphere/rbnacl) which is based of [NaCl](http://nacl.cr.yp.to/).

Use the [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi) buildpack and add this buildpack to your `.buildpacks` file.


And set LD_LIBRARY_PATH

```
heroku config:set LD_LIBRARY_PATH=/app/vendor/libsodium-0.4.5/src/libsodium/.libs
```
