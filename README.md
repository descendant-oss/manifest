Descendant specificity document

https://docs.google.com/document/d/1VnGGvwlsvM_9d2IzJn_D4Us55f8G6FgOd3NnsrkN8og/edit?usp=sharing

To initialize your local repository, use this command:

	repo init -u https://github.com/descendant-oss/manifest -b eleven-staging

 Then to sync up:

```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```

Build Descendant
==================

```bash
source build/envsetup.sh

lunch descendant_codename-buildtype

mka descendant
```
