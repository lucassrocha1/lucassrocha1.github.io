# Xolingo content CDN

Served content for the [Xolingo](https://github.com/lucassrocha1) app's
content CDN client (`app_flutter/lib/data/content_repository.dart`).

**Generated output — do not hand-edit.** `catalog.json` is produced by
`tools/curate_texts.py` in the Xolingo repo and copied here. To publish an
update:

```sh
cd xolingo/tools
python3 curate_texts.py --out ../app_flutter/assets/content/catalog.json
cp ../app_flutter/assets/content/catalog.json /path/to/lucassrocha1.github.io/xolingo/catalog.json
cd /path/to/lucassrocha1.github.io && git add -A && git commit -m "Update Xolingo content catalog" && git push
```

`catalogVersion` is a `YYYYMMDD` integer, so any later publish is
automatically picked up by clients — no manual bump needed.

Live at: `https://lucassrocha1.github.io/xolingo/catalog.json`
