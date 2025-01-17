# Usefull VS Code Keyboard Shortcuts

As seen on Wes Bos' YT video.

## Navigation based on cursor position

`Ctrl + -` will go back in history through open files where your cursor were

## Jump to last edit location

`Cmd + K, Cmd + Q` will take you to last edit location

## Navigate through tabs based on recent locations

`Ctrl + Tab` will take you to the previous tab. If you hold it, you'll get a list of tabs sorted by recency. By tapping it quickly you'll be able to switch between last two used really quickly.

`Cmd + p + p` does the same thing apparently.

## Goto symbol

First tap `Cmd + p` to open file search. Then if you type `@` you'll get a list of symbols in the current file. Symbols are methods, properties, CSS class definitions or whatnots depending on file type.
By adding `:` after `@` you'll get them sorted (`@:`). Of course, you can continue with the fuzzy search after the `@` to find a method you are looking for.

This not only works in the current file but across the workspace. So `Cmd + p` then start typing file name followed by `@` and you'll get symbols for the first file from the search.

## Quick text search

Tap `Cmd + p` and then enter `%` and you'll be able to do a quick text search across your workspace and if you scroll (with keyboard) through the list you'll get a quick preview of the found text in the file itself.

## Goto definition

Hold `Cmd` and then click on the method name and you'll be taken to its definition.

Subsequently, if you are on method declaration line and click `F12` (mind the `Fn` key) you'll get a "peaker" with a list of files and lines where the method is being called from.

## Move or select by word

If you use `Alt/Option + left or right arrow` you'll move either by symbol or string. But if you add `Ctrl` in the mix (`Ctrl + Alt/Option + left or right arrow`) you'll move by word even in camel case or snake case.

[Source](https://www.youtube.com/watch?v=c0HO_-NDJCk)