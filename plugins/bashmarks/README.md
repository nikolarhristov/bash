# Bashmarks plugin

The Bashmarks plugin allows you to create and use bookmarks for directories on
your filesystems. This plugin is derived from the project
HTTPS://github.com/huyng/bashmarks but contains improvements.

## Quickstart

Create a new bookmark using the _bm -a_ command:

```bash
$ bm -a mydir
```

The command above creates a bookmark for the current directory with the name
_mydir_.

You can navigate to the location of a bookmark using the _bm -g_ command:

```bash
$ bm -g mydir
```

You can also supply just any bookmark name and the _-g_ option will be assumed:

```bash
$ bm mydir
```

Tab completion is available when you need to enter a bookmark name in a command,
such as when using _bm -g_

Easily list all bookmarks you have set up using the _bm -l_ command:

```bash
$ bm -l
```

## Configuration

-   **`BASHMARKS_SDIR`**: This variable contains the path to the file that
    stores the information of bookmarks of directory names. The default path is
    `~/.sdirs`. The old interface `SDIRS` is now deprecated.

## Commands

-   **`bm -h`**: Print short help text
-   **`bm -a bookmarkname`**: Save the current directory as bookmarkname
-   **`bm [-g] bookmarkname`**: Go to the specified bookmark
-   **`bm -p bookmarkname`**: Print the bookmark
-   **`bm -d bookmarkname`**: Delete a bookmark
-   **`bm -l`**: List all bookmarks

## Valid bookmark names

A bookmark name can contain lower and upper case characters (A-Z), numbers and
underscore characters. No periods, semicolons, spaces or other characters are
allowed in a bookmark name.
