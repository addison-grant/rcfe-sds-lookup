# Chemical safety sheets

A phone-friendly lookup page for the safety data sheets (SDS) of the chemicals we use. Staff can search a product to see first aid, protective gear, spill cleanup and storage rules, and open the full SDS.

## Adding or changing a product

All products live in `products.json`. To add one, copy an existing entry, change the fields, and commit. The site updates a minute or two later.

- `id`: lowercase words with dashes, unique (used in the link, e.g. `#p-clorox-regular-bleach`)
- `signal`: `Danger`, `Warning`, `Caution`, or `None`
- `hazards`, `ppe`, `spill`, `storage`, `mixing`: lists of short lines
- `firstAid`: `eyes`, `skin`, `inhaled`, `swallowed`
- `house`: our facility's own rule (optional)
- `sdsDate`, `sdsUrl`, `makerPhone`, `sourceNote`: where the info came from

The summaries help staff find things fast. They do not replace the full SDS, which must still be kept on file and available to staff on every shift.
