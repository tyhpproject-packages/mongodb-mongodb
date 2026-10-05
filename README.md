<!-- tyhp-readme:start -->
# tyhpdef/mongodb-mongodb

Tyhp type definitions for `mongodb/mongodb` `2.4.2`.

```bash
composer require --dev tyhpdef/mongodb-mongodb:2.4.2
```

This is a metapackage. Composer also installs `tyhpdef/mongodb-mongodb-impl` (type files).
Require **this** name, not `tyhpdef/mongodb-mongodb-impl`.

See https://tyhplang.com.

## Maintain `mongodb/mongodb`? Ship the types yourself

If you are a Packagist maintainer of `mongodb/mongodb`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/mongodb-mongodb-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `mongodb/mongodb` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/mongodb-mongodb": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `mongodb/mongodb` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `mongodb/mongodb` with a real constraint,
   `"replace": { "tyhpdef/mongodb-mongodb": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `mongodb/mongodb` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/mongodb-mongodb` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
