# myanmar-burmese-legacy-fonts

Legacy Myanmar (Burmese) fonts, gathered from several public sources into one
place, so anyone working with Burmese text can download and use them. Win
Metta compiled it on 2026-11-26.

"Legacy" here means fonts that are **not Unicode**: the Zawgyi-One family and
its many look-alikes (Zawgyi encoding) and the Win Innwa / "Win" font family
(a different, older encoding). Old documents, web pages, PDFs and chat logs
written in these encodings only display correctly with a matching font, and
show as garbled text in Unicode-aware software. Installing the right font here
is the way to read them, and a converter (Zawgyi to Unicode, for example) is
the way to rescue the text. Some collections also contain Unicode fonts
(Padauk, Pyidaungsu, Noto Sans Myanmar, Myanmar Text and others), which are
kept as they came.

## How to use

- Download only the font file you need, not the whole repository (it is
  large). On GitHub, open the `.ttf` file and use **Download raw file**.
- Not sure which font a document uses? Look in [`dafontfree.net/`](dafontfree.net/) for the Win
  fonts and in [`KhunHtetzNaing-AllZawgyiFont/z/Myanmar/Zawgyi/`](KhunHtetzNaing-AllZawgyiFont/z/Myanmar/Zawgyi/) for Zawgyi
  fonts, and try a few until the text is readable.
- Install the font as usual on your system. On macOS, see the Zawgyi guide in
  [`aungthumoe5-zawgyi-on-mac/`](aungthumoe5-zawgyi-on-mac/README.md).
- For anything new, write in Unicode (Myanmar block U+1000 to U+109F), such as
  Padauk, Pyidaungsu or Noto Sans Myanmar. Win Metta's own content is always
  Unicode and never Zawgyi.

## Find a font

[`FONTS.md`](FONTS.md) lists every font in the repository, grouped by kind
(Zawgyi, the Win family and its sub-groups, Unicode and others). Each unique
font appears once, with all the files that hold the same content, even when
they come from different sources or have different file names.

## Sources at a glance

| Directory                                                                      | Obtained as                         | Upstream                                                                                              | TTF files         | Size   |
| ------------------------------------------------------------------------------ | ----------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------- | ------ |
| [`dafontfree.net/`](dafontfree.net/)                                           | 58 zips downloaded from the website | [dafontfree.net search "wininnwa"](https://www.dafontfree.net/search?key=wininnwa&alias=fonts&page=1) | 59                | 4.7 MB |
| [`swanbros-free-myanmar-burmese-fonts/`](swanbros-free-myanmar-burmese-fonts/) | One zip downloaded from a URL       | [free-myanmar-burmese-fonts.softag.com](https://free-myanmar-burmese-fonts.softag.com/)               | 20                | 3.5 MB |
| [`KhunHtetzNaing-AllZawgyiFont/`](KhunHtetzNaing-AllZawgyiFont/)               | GitHub repository                   | [KhunHtetzNaing/AllZawgyiFont](https://github.com/KhunHtetzNaing/AllZawgyiFont)                       | 187 (+1 OTF)      | 144 MB |
| [`moekyawsoe-Myanmar-Fonts/`](moekyawsoe-Myanmar-Fonts/)                       | GitHub repository                   | [moekyawsoe/Myanmar-Fonts](https://github.com/moekyawsoe/Myanmar-Fonts)                               | 321 (plus 60 OTF) | 34 MB  |
| [`aungthumoe5-zawgyi-on-mac/`](aungthumoe5-zawgyi-on-mac/)                     | GitHub repository                   | [aungthumoe5/zawgyi-on-mac](https://github.com/aungthumoe5/zawgyi-on-mac)                             | 7                 | 3.8 MB |

Each directory is a copy of its source, kept as close to the original as
possible (the GitHub directories are named `<owner>-<repo>`), so upstream README
files are kept inside them. Only font files are kept: non-font files, archives
and same-name duplicates were removed, as described in each directory's README.
Stated licences are in [Licence notes](#licence-notes-from-the-sources).

## Source details

### `dafontfree.net/`

The 58 fonts that DafontFree returns for the search key `wininnwa`, mostly the
Win Innwa family and related "Win" and "WWin" fonts, plus Zawgyi-One Regular.
Each font page's **Download zip** button was used, and only the `.ttf` files
were extracted. [`dafontfree.net/README.md`](dafontfree.net/README.md) lists
every file with its font page link. The pages say "Download free for Personal
Use".

### `swanbros-free-myanmar-burmese-fonts/`

The "Myanmar Language Sources Package" by Swanbros, labelled freeware,
updated 2019-02-24 on the download page, with fonts dated 2007. It holds 20
TrueType fonts (Myanmar1, Myanmar2, Win Innwa, Win Hlaing, Win Yadanapon,
Zawgyi One 2007 and others) and their Type 1 versions (`.pfb`/`.pfm`, 41
pairs), plus a PDF typing guide and a keyboard layout image. This is the
original zip contents, so there is no upstream git history.

### `KhunHtetzNaing-AllZawgyiFont/`

A large collection by KhunHtetzNaing, last pushed upstream on 2019-07-24, with
no licence. It contains:

- About 40 Zawgyi display fonts in [`z/Myanmar/Zawgyi/`](KhunHtetzNaing-AllZawgyiFont/z/Myanmar/Zawgyi/) (the repository root
  held a second copy of 39 of them, now removed, see
  [Duplicates](#duplicates)), plus Noto Sans Zawgyi in several web formats.
- [`z/Myanmar/Unicode/`](KhunHtetzNaing-AllZawgyiFont/z/Myanmar/Unicode/): 78 Unicode Myanmar fonts (the
  `Unicode.zip` that duplicated them was removed).
- [`z/Colored/`](KhunHtetzNaing-AllZawgyiFont/z/Colored/), [`z/Cool/`](KhunHtetzNaing-AllZawgyiFont/z/Cool/), [`z/Emojis/`](KhunHtetzNaing-AllZawgyiFont/z/Emojis/): 65 colour, decorative and emoji fonts
  that are not Burmese fonts.
- [`from-myZawgyiFont.zip/`](KhunHtetzNaing-AllZawgyiFont/from-myZawgyiFont.zip/): two fonts (`dancing.ttf`, `tabodwe mix.ttf`)
  rescued from the upstream's `myZawgyiFont.zip`, which was removed (see
  [Files removed](#files-removed-fonts-only)).
- `index.html`: a font-face demo that loads fonts from a CDN.

### `moekyawsoe-Myanmar-Fonts/`

A Windows-oriented bundle by moekyawsoe, last pushed upstream on 2019-06-05,
with no licence:

- Loose fonts: Myanmar Text (`MMRTEXT`), Padauk, Pyidaungsu 2.5.2, Zawgyi-One
  v3.1, WinInnwa and others (11 TTFs).
- [`Myanmar Fonts TTF Series 2/`](moekyawsoe-Myanmar-Fonts/Myanmar%20Fonts%20TTF%20Series%202/) (extracted from the upstream's rar): 310
  TTFs, 60 OTFs, and Type 1 files.
- Three further archives (Zawgyi installers and a cracked WinRAR) were
  removed (see [Files removed](#files-removed-fonts-only)).

### `aungthumoe5-zawgyi-on-mac/`

A guide to using Zawgyi on macOS, by aungthumoe5, last pushed upstream on
2018-09-23, MIT licensed. It contains three Zawgyi-One TTFs, Padauk 3.003
(extracted to [`Fonts/Padauk/padauk-3.003/`](aungthumoe5-zawgyi-on-mac/Fonts/Padauk/padauk-3.003/), SIL Open Font Licence). Upstream
also shipped the Ukelele 3.2.3 keyboard
editor (`.dmg`), which was removed here. Upstream's default branch is
`master`.

## Files removed (fonts only)

This repository tracks fonts only. These file types from the original sources
were deleted from this copy because they are not fonts and could harm people
who download and run them: `.exe`, `.msi`, `.dll`, `.apk`, `.dmg`,
`.mobileconfig` and `.reg`, and the archives that contained them. In total 45
files were removed, plus the whole `iOS/` page described below:

- `KhunHtetzNaing-AllZawgyiFont/iOS/`: the 39 `.mobileconfig` iOS font
  profiles and the upstream's web page for downloading them (HTML, CSS,
  JavaScript and icon fonts, no Burmese fonts). The whole directory was
  removed.
- `aungthumoe5-zawgyi-on-mac/Keyboard Editor/Ukelele_3.2.3.dmg`.
- `moekyawsoe-Myanmar-Fonts/fonts.reg`.
- `moekyawsoe-Myanmar-Fonts/zawgyi_fonts_installer.rar` and
  `IEZawGyiGtalkfont.rar` (installers), and `WinRAR 3.51.rar` (WinRAR with a
  licence bypass).
- `KhunHtetzNaing-AllZawgyiFont/myZawgyiFont.zip` (12 APKs plus 39 TTFs; the
  only two TTFs without an identical copy elsewhere were kept in
  [`from-myZawgyiFont.zip/`](KhunHtetzNaing-AllZawgyiFont/from-myZawgyiFont.zip/)).

Each affected directory's README lists what was removed.

The remaining three archives were extracted and then deleted, since they held
only fonts and documentation: `Unicode.zip` (all of its fonts already existed
unpacked, so nothing was extracted), `padauk-3.003.zip` and
`Myanmar Fonts TTF Series 2.rar`. The repository now contains no `.zip` or
`.rar` files.

## Malware scan

After the cleanup the repository was scanned once with ClamAV: 0 infected files.
Details are in [`clamav-scan.md`](clamav-scan.md).

## Notes

1. **Off-topic fonts.** The 65 colour, decorative and emoji fonts in
   KhunHtetzNaing [`z/Colored`](KhunHtetzNaing-AllZawgyiFont/z/Colored/), [`z/Cool`](KhunHtetzNaing-AllZawgyiFont/z/Cool/) and [`z/Emojis`](KhunHtetzNaing-AllZawgyiFont/z/Emojis/) are not Burmese fonts.
2. **Size.** About 190 MB of binaries is a lot for plain git. Consider Git LFS
   or a release download.

### Duplicates

Within each source, a file counts as a duplicate when another file has the same
name and byte-identical contents (SHA-256). Those were removed, keeping one
copy:

- `KhunHtetzNaing-AllZawgyiFont`: 39 fonts that appeared in both the root and
  [`z/Myanmar/Zawgyi/`](KhunHtetzNaing-AllZawgyiFont/z/Myanmar/Zawgyi/) (root copies deleted).
- No duplicates in the other four sources.

Kept on purpose, because people find fonts by name: files with identical
contents but different names, such as `ZawgyiOne2005.ttf`/`ZawgyiOne2008.ttf`,
`Thanlwin-Bold.ttf`/`Thanlwin-Regular.ttf` and
`MyanmarText_Bold.ttf`/`MyanmarText_Regular.ttf` (the Bold files are probably
an upstream mistake and not really bold), and `WW_BURN0.TTF`/`ww_burn4.ttf`.
Duplicates **across** sources were not removed, so the same font can appear in
two directories (for example `WININNWA.TTF`, `Wininnwa.ttf` and
`wininnwa.ttf`, and the three Zawgyi-One 2005 to 2008 files).

## Licence notes from the sources

What each source states about licensing, kept as provenance. These are legacy
fonts that were widely used across Burmese websites, collected here for anyone
working with Burmese text.

| Source                                                                         | Stated licence                                                                 |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| [`dafontfree.net/`](dafontfree.net/)                                           | "Download free for Personal Use" on each font page                             |
| [`swanbros-free-myanmar-burmese-fonts/`](swanbros-free-myanmar-burmese-fonts/) | "Freeware" (download page)                                                     |
| [`KhunHtetzNaing-AllZawgyiFont/`](KhunHtetzNaing-AllZawgyiFont/)               | None stated                                                                    |
| [`moekyawsoe-Myanmar-Fonts/`](moekyawsoe-Myanmar-Fonts/)                       | None stated                                                                    |
| [`aungthumoe5-zawgyi-on-mac/`](aungthumoe5-zawgyi-on-mac/)                     | MIT for the repository; Padauk is SIL OFL 1.1; Zawgyi and Ukelele are separate |

## Adding a source

1. Put it in its own top-level directory: `<github-owner>-<repo>` for a
   GitHub repository, or the website or vendor name for a download.
2. Keep a copy of what was downloaded, including its README.
3. Add a row to [Sources at a glance](#sources-at-a-glance) and a section
   under [Source details](#source-details) with the URL, the date obtained
   and the licence.
