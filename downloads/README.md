# Put your app file here

Drop your Android **`.apk`** (or any installer file) into this folder and name it
`myapp.apk` — that's the filename the download button on the site points to.

If you use a different name, update the `href` in `index.html`:

```html
<a class="download-btn" href="downloads/YOUR-FILE.apk" download>
```

## ⚠️ File size note
GitHub blocks files larger than **100 MB**. If your APK is bigger than that:
- Use [Git LFS](https://git-lfs.com/), **or**
- Host the file elsewhere (e.g. a release asset or cloud storage) and point the
  button's `href` at that URL instead.
