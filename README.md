# Chore Factory

by Ben Winchester, Rural Sociologist. November, 2026.

A home maintenance and household inventory tracker: chores on a schedule,
an inventory drawn on a house diagram, and recall findings for each item.

The page runs on GitHub Pages. Everything it stores is in `data.enc`, locked
with AES-GCM in the browser before it is saved; the key travels only in the
owner's link (`#k=...`) and is never sent here. Without the key the file is
unreadable.

`nextup.json` is the one plain file: the jobs coming due, read by a kitchen
display. It holds task names, item names and dates, nothing else.

Saving from a device needs a fine-grained GitHub token that can write to this
repository's contents, entered once in the page and kept in that browser.
