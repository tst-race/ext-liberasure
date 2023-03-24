# liberasurecode for RACE

This repo provides scripts to custom-build the
[liberasurecode library](https://github.com/openstack/liberasurecode) for RACE.

## License

The liberasurecode library is licensed under the 3-Clause BSD license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

liberasurecode has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build liberasurecode.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-liberasurecode.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-liberasurecode
```

## Platforms

liberasurecode is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`
* `android-x86_64`
* `android-arm64-v8a`

## How It Is Used

liberasurecode is used by slothy.
