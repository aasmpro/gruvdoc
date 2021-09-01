### Made with
an extra `made_with` key can change `Made with ...` content in footer.
- set `true` to show default
- set `false` or comment to remove
- or set your custom text!

```yaml
extra:
    made_with: true # or false
    # or
    made_with: Made with Love!
```

### Version
an extra `version` key can version content in footer.
```yaml
extra:
    version:
        name: v1.0.0
        link: https://github.com/aasmpro/gruvdoc/releases/tag/v1.0.0
```

### License
an extra `license` key can version content in footer.
```yaml
extra:
    license:
        name: GPL3+
        link: https://github.com/aasmpro/gruvdoc/blob/master/LICENSE
```

### Sortable tables
`tablesort.js` file in extra javascript files contains the code which make table headers clickable for sorting.