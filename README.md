# readerisdead.com

A collection of tools to help with the [Google Reader shutdown](http://googlereader.blogspot.com/2013/07/a-final-farewell.html).

## reader_browser

_Browse an archived Google Reader account._

Takes an archive generated by `reader_archive` and provides a browsing UI for it.

To use it:

```
bin/reader_browser ~/Downloads/reader_archive
```

Then you can load http://localhost:8071/ in your web browser to see the contents of the archive.

## item_lookup

_Look up an item in an archived Google Reader account._

Takes an archive generated by `reader_arhive` and provides a command-line UI for examining items within it.

To use it:

```
bin/item_lookup --archive_directory=~/Downloads/reader_archive 0306277b9d275db1
```

The tool will then list all of the streams that the item appears in, the item body, and any comments made on that item. You can provide multiple item IDs (as additional command line arguments).

## Archived Tools

Now that Google Reader has been shut down, some of the initial tools (focused on getting the data out) are no longer useful. They were:

* [`reader_archive`](https://github.com/mihaip/readerisdead/wiki/reader_archive): Saved a comprehensive archive of a Google Reader account.
* [`feed_archive`](https://github.com/mihaip/readerisdead/wiki/feed_archive): Saved public feed data from Google Reader's feed cache.
