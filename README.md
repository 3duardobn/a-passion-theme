# A Passion — theme for Firefox-based browsers

Port of the **A Passion** theme (Chrome Web Store) to any Firefox-based
browser — Firefox, Zen, Waterfox, Floorp and others — plus a matching
**Sidebery** theme.

It uses `userChrome.css` and `userContent.css`, so there is no extension and
no signed theme to install.

![A Passion](browser/chrome/a-passion/ntp.png)

- Original theme: **A Passion** by **Abelle Hayford** — [abellehayford.com](https://abellehayford.com/)
- Chrome Web Store: [chromewebstore.google.com/detail/a-passion](https://chromewebstore.google.com/detail/a-passion/elbejlmapdnkbjofccadjlkmcpggfclg)

## Colors

| Use | Hex |
| --- | --- |
| Frame / panel | `#1a1a51` |
| Toolbar / active tab | `#323fa6` |
| Accent (pink) | `#de6af0` |
| Focus / search | `#68d3ef` |
| Popups / menus | `#12123a` |
| Raised elements | `#24245f` |
| Text | `#ffffff` |

## Files

```text
browser/chrome/
├── userChrome.css              # imports the browser theme
├── userContent.css             # imports the new tab theme
└── a-passion/
    ├── a-passion.css           # tabs, toolbars, menus, sidebar
    ├── newtab.css              # new tab layout
    ├── ntp-data.css            # artwork embedded as a data: URL
    └── ntp.png                 # original 1920×1080 artwork
sidebery/
└── a-passion-sidebery.css      # Sidebery theme
```

## Install

1. Copy the contents of `browser/chrome/` into your profile's `chrome/` folder
   (`about:profiles` shows the path).
2. In `about:config`, set
   `toolkit.legacyUserProfileCustomizations.stylesheets = true`.
3. Close **all** browser windows and open the browser again — `userChrome.css`
   is only read at startup.

Sidebery: open **Settings → Styles → Styles editor**, paste
`sidebery/a-passion-sidebery.css` and save.

## License

The **code** (CSS, HTML and scripts in this repository) is in the **public
domain**, under the [Unlicense](LICENSE).

The **artwork and visual identity** of the original theme belong to **Abelle
Hayford** and are used here for personal use only, with credit. See
[NOTICE.md](NOTICE.md).
