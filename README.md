# easyDialog (RaP-SoR / open.mp)

Fork of [devbluen/easyDialog](https://github.com/devbluen/easyDialog) with open.mp / modern `pawncc` packaging.

Upstream `1.0.4` brings input/listitem protections and `Dialog_ReShow`.
This fork adds compiler-clean fixes so consumers do not need post-`ensure` local patches.

## Install (sampctl)

```
sampctl install RaP-SoR/easyDialog:1.1.0
```

Requires YSI (`y_hooks`, `y_va`). Include YSI **before** `<easyDialog>`.

## open.mp fixes (vs upstream 1.0.4)

- Forward declarations for tagged returns (`bool:`, `DIALOG_STYLE:`)
- Renamed shadowed locals (`status` → `created_status`, `string` → `haystack`)

## Credits

- Emmet_ / Awsomedude — original idea
- devonblue — protections and `Dialog_ReShow`
- RaP-SoR — open.mp sampctl packaging
