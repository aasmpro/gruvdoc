### Sortable tables
`tablesort.js` file in extra javascript files contains the code which make table headers clickable for sorting.

!!! note
    style fixes are done with utils file.

### Task list color
setting task list checked item color to theme `--md-primary-fg-color`.

### Selection color
this part sets user selection foreground color to `--md-default-fg-color` and background to `--md-typeset-mark-color` from current theme.

### Search placeholder color
by default search place holder color wont change with changing theme for scheme, here placeholder color sets to theme `--md-default-fg-color`.

### Table header
table headers like placeholders wont change with theme colors, so GruvDoc set foreground color to `--md-default-fg-color` and background to `--md-primary-fg-color` from current theme .

### Remove footer
if you want to remove footer entirely, uncomment styles for `.md-footer`.