<!-- tyhp-readme:start -->
# tyhpdef/symfony-config

Tyhp type definitions for `symfony/config` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-config:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-config-impl` (type files).
Require **this** name, not `tyhpdef/symfony-config-impl`.

See https://tyhplang.com.

## Maintain `symfony/config`? Ship the types yourself

If you are a Packagist maintainer of `symfony/config`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-config-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/config` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-config": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/config` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/config` with a real constraint,
   `"replace": { "tyhpdef/symfony-config": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/config` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-config` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
