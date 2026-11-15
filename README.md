# laoshi-stroke-data

Stroke-order data used by the Laoshi iOS app's Write It stage.

## Source and license

Derived from [Make Me a Hanzi](https://github.com/skishore/makemeahanzi), through the
[hanzi-writer-data](https://github.com/chanind/hanzi-writer-data) package (version 2.0.1).

Copyright 1999 Arphic Technology Co., Ltd.; copyright 2016 Shaunak Kishore.
Licensed under the **Arphic Public License** (see `ARPHICPL.TXT`, included unaltered).
You may copy, modify and redistribute this data under that license.

## Changes (14 November 2026)

`laoshi-strokes-v1.json` is a modified version of the source data:

- Only the 238 characters taught in Laoshi are included.
- Only stroke medians (centre lines) are kept. Outlines are dropped.
- Coordinates are converted from the 1024-unit font box (y up, baseline 900) to 0..1 with y down, and rounded to 3 decimals.
- Each stroke has a short spoken description added for VoiceOver.

The file is built by `scripts/generate-stroke-data.py` in the Laoshi app repository.
