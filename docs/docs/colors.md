GruvDoc supports all [GruvBox](https://github.com/morhetz/gruvbox) colors for both `primary` and `accent` color.

you must set theme to `material` and palette scheme to `gruvbox`:
```yaml hl_lines="2 4"
theme:
  name: material
  palette:
    scheme: gruvbox
    primary: green
    accent: green
```

color names for primary and accent colors:

| Default                      | *1                            | *2                            |
| ---------------------------- | ----------------------------- | ----------------------------- |
| gray { .bg-color-gray0 }     | gray1 { .bg-color-gray1 }     | gray2 { .bg-color-gray2 }     |
| red { .bg-color-red0 }       | red1 { .bg-color-red1 }       | red2 { .bg-color-red2 }       |
| green { .bg-color-green0 }   | green1 { .bg-color-green1 }   | green2 { .bg-color-green2 }   |
| yellow { .bg-color-yellow0 } | yellow1 { .bg-color-yellow1 } | yellow2 { .bg-color-yellow2 } |
| blue { .bg-color-blue0 }     | blue1 { .bg-color-blue1 }     | blue2 { .bg-color-blue2 }     |
| purple { .bg-color-purple0 } | purple1 { .bg-color-purple1 } | purple2 { .bg-color-purple2 } |
| aqua { .bg-color-aqua0 }     | aqua1 { .bg-color-aqua1 }     | aqua2 { .bg-color-aqua2 }     |
| orange { .bg-color-orange0 } | orange1 { .bg-color-orange1 } | orange2 { .bg-color-orange2 } |

!!! quote "Black theme"
    there is also a `black` theme for primary which is configured with `blue` accent.

!!! note
    scheme, primary and accent css files exist in `/docs/assets/stylesheets/`


## Palette
color palette variables are in `/docs/assets/stylesheets/vars.css`. there are 11 variables per color, starting with `--color-` prefix then color name and for shades `--color-[color-name]-rgba[opacity]`. an example for red color:
```css
:root {
    /* Red0 */
    --color-red0: #9d0006;
    --color-red0-rgba10: rgba(157, 0, 6, 1);
    --color-red0-rgba09: rgba(157, 0, 6, 0.9);
    --color-red0-rgba08: rgba(157, 0, 6, 0.8);
    --color-red0-rgba07: rgba(157, 0, 6, 0.7);
    --color-red0-rgba06: rgba(157, 0, 6, 0.6);
    --color-red0-rgba05: rgba(157, 0, 6, 0.5);
    --color-red0-rgba04: rgba(157, 0, 6, 0.4);
    --color-red0-rgba03: rgba(157, 0, 6, 0.3);
    --color-red0-rgba02: rgba(157, 0, 6, 0.2);
    --color-red0-rgba01: rgba(157, 0, 6, 0.1);
}
```

| color names                                    |
| ---------------------------------------------- |
| black, white                                   |
| dark0, dark1, dark2, dark3, dark4, dark5       |
| light0, light1, light2, light3, light4, light5 |
| gray0, gray1, gray2                            |
| red0, red1, red2                               |
| green0, green1, green2                         |
| yellow0, yellow1, yellow2                      |
| blue0, blue1, blue2                            |
| purple0, purple1, purple2                      |
| aqua0, aqua1, aqua2                            |
| orange0, orange1, orange2                      |


## Admonitions
[admonitions](/gruvdoc/demo/admonitions/) colors are configured in `/docs/assets/stylesheets/admonitions.css`.