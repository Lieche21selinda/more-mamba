# GitHub upload — flat version

Every file in this folder sits at the top level. There are no subfolders, and
`index.html` points at the images directly (`portrait-formal.jpg`, not
`assets/portrait-formal.jpg`).

That is deliberate. Your last upload flattened the `assets` folder, so the images
landed at the root while `index.html` was still looking for them inside `assets/`.
Hence the broken-image icons. This version cannot hit that problem, because there
is no folder to flatten.

## What to do

1. Unzip this file.
2. Go to https://github.com/lieche21selinda/masego-website-NWU
3. Delete everything currently in the repository. Quickest route: **Settings** →
   scroll to the bottom → **Delete this repository** → then create a new one with
   the same name. Otherwise delete each file individually.
4. **Add file** → **Upload files**.
5. Select all the files from step 1 and drag them in. Order does not matter, and
   they can go in more than one batch if the browser struggles — there are 41.
6. **Commit changes**.
7. **Settings** → **Pages** → Source: *Deploy from a branch*, Branch: **main**,
   Folder: **/ (root)** → **Save**.
8. Give it two or three minutes.

Nothing should be inside a folder when you are done. `index.html` and all the
`.jpg` files sit side by side in the repository root.

## Check it worked

Open the site and click through to the **Evidence index** slide, then click one of
the STLES entries. If the image opens full size, everything is wired up.

If images are still broken, right-click one → **Open image in new tab** and look at
the address. It tells you exactly which filename the page is asking for and where
it expects to find it.

## Note

This is the GitHub copy. Keep `mokgoko-portfolio.zip` for editing — it has the
tidier `assets/` folder and the PDF build script. If you change the deck there and
want to republish, tell me and I will regenerate this flat version.
