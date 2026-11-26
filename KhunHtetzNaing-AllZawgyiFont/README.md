# AllZawgyiFont

Zawgyi Font Collections

Source: <https://github.com/KhunHtetzNaing/AllZawgyiFont>

---

## Files removed from this copy (Win Metta)

This repository tracks fonts only, so these files from the original source were
deleted from this copy:

- `iOS/`: the whole directory. It held 39 Apple `.mobileconfig` profiles that
  install a font on an iPhone or iPad (the matching TTFs are in
  [`z/Myanmar/Zawgyi/`](z/Myanmar/Zawgyi/)), plus the upstream's download page
  for them: one HTML file, 4 CSS and 4 JavaScript files, and the page's
  icon fonts and images (no Burmese fonts).

- `myZawgyiFont.zip`: 12 Android APKs (each installing one font) and 39 TTFs.
  The TTFs duplicate fonts already in this directory, except two whose bytes
  differ from every other copy: `dancing.ttf` and `tabodwe mix.ttf`. Those two
  were extracted to [`from-myZawgyiFont.zip/`](from-myZawgyiFont.zip/) before the archive was deleted.

- `z/Myanmar/Unicode/Unicode.zip`: its 76 TTFs were already extracted
  next to it in [`z/Myanmar/Unicode/`](z/Myanmar/Unicode/) with identical contents, so the zip was
  simply deleted. Nothing was extracted from it.

## Duplicates removed from this copy (Win Metta)

39 fonts existed twice, once in the repository root and once in
[`z/Myanmar/Zawgyi/`](z/Myanmar/Zawgyi/), with identical contents (SHA-256) and the same file name.
The root copies were deleted and the [`z/Myanmar/Zawgyi/`](z/Myanmar/Zawgyi/) copies kept:
`dancing`, `dc`, `eainmat`, `ghost`, `heart`, `htinshu`, `izawgyi`, `jojar`,
`kason`, `khnisi`, `love`, `matrix`, `nattaw`, `nayon`, `ngaye`, `notosans`,
`notosansmix`, `ooredoo`, `padauk`, `pyatho`, `sagar`, `szg`, `tabaung`,
`tabodwemix`, `tagu`, `tbd`, `tdg`, `tran`, `tsm`, `ttl`, `ubuntu`, `warso`,
`wg`, `yoeyar`, `yuzana`, `z2`, `zo`, `zy` and `paoh` (all `.ttf`). The
root keeps only the `.ttf` copies of `NotoSansZawgyi`, `mon3` and `paoh_zg`; the
web-font copies of those fonts (`.eot`, `.otf`, `.svg`, `.woff`, `.woff2`) and
`zawgyi.woff` stay beside them.

Files with identical contents but different names were **kept**, because
people look fonts up by name: `Thanlwin-Bold`/`Thanlwin-Regular`,
`MyanmarText_Bold`/`MyanmarText_Regular` and `MonAnonta`/`mon3` (all in
[`z/Myanmar/Unicode/`](z/Myanmar/Unicode/)).
