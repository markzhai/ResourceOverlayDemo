# ResourceOverlayDemo

Demo to show Android aapt overlay and gradle resource merge

## aapt Overlay

Show how to apply overlay resource directory in gradle-based build system.

```bash
Usage:
 aapt l[ist] [-v] [-a] file.{zip,jar,apk}
   List contents of Zip-compatible archive.

 aapt d[ump] [--values] [--include-meta-data] WHAT file.{apk} [asset [asset ...]]
   ...

 aapt p[ackage] [-d][-f][-m][-u][-v][-x][-z][-M AndroidManifest.xml] \
        ...
        [--utf16] [--auto-add-overlay] \
        ...
        [-S resource-sources [-S resource-sources ...]] \
        [-F apk-file] [-J R-file-dir] \
        ...

   Package the android resources.  It will read assets and resources that are
   supplied with the -M -A -S or raw-files-dir arguments.  The -J -P -F and -R
   options control which files are output.

...

 Modifiers:
   ...
   -I  add an existing package to base include set
   ...
   -S  directory in which to find resources.  Multiple directories will be scanned
       and the first match found (left to right) will take precedence.
   ...
   --auto-add-overlay
       Automatically add resources that are only in overlays.
   ...
```

## gradle resource merge

http://tools.android.com/tech-docs/new-build-system/resource-merging
