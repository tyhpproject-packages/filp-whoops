<!-- tyhp-readme:start -->
# tyhpdef/filp-whoops

Tyhp type definitions for `filp/whoops` `2.18.4`.

```bash
composer require --dev tyhpdef/filp-whoops:2.18.4
```

This is a metapackage. Composer also installs `tyhpdef/filp-whoops-impl` (type files).
Require **this** name, not `tyhpdef/filp-whoops-impl`.

See https://tyhplang.com.

## Maintain `filp/whoops`? Ship the types yourself

If you are a Packagist maintainer of `filp/whoops`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/filp-whoops-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `filp/whoops` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/filp-whoops": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `filp/whoops` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `filp/whoops` with a real constraint,
   `"replace": { "tyhpdef/filp-whoops": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `filp/whoops` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/filp-whoops` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
