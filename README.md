# VRM eReader public-domain test content

This folder contains Agrippa Book I chapter text and linked notes from the 1913
*Philosophy of Natural Magic*, downloaded from Global Grey. It excludes the
publisher's front matter and Morley/De Laurence end matter. This is a development
acceptance fixture; curate the production edition separately.

Upload the CONTENTS of this folder to your repository's published directory:

    .nojekyll
    README.md
    155/
      book.json
      curation.json
      images/
        img-...-pc.jpg
        img-...-mobile.jpg

Keep the filenames unchanged. book.json references the image filenames relative
to itself. curation.json records the processor choices and can be retained for
reproducibility. There are 74 generated chapter sections, one title section,
32 linked note sections and nine source illustrations (two platform files each).
These generated labels are not printed-page numbers.

Enable GitHub Pages for that directory. For a repository called REPO belonging
to OWNER, the usual public base is https://OWNER.github.io/REPO/ and this manifest
is https://OWNER.github.io/REPO/155/book.json . Confirm both the manifest and an
image are accessible directly, without a login or redirect.

Unity LibrarySystem_v2.contentBase: https://OWNER.github.io/REPO/
Catalog book ID 155: add eReaderURL with the value 155/book.json .
Preserve the catalog's existing url field (it is a separate external/store link).
Build & Test and upload both prepare the serialized URL table automatically.

The original EPUB and all supplied Hermes files are intentionally absent. Nothing
in this tooling publishes or uploads files automatically.
