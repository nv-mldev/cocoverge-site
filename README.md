# cocoverge.in

Deployed copy of the CocoVerge one-page site, served by GitHub Pages.

Source of truth is `current/website/` in the private radhus folder. Do not edit here.
To publish a change: edit the source, then run from the radhus folder:

    rsync -a --delete --exclude .git --exclude .DS_Store --exclude REVIEW.md current/website/ ../cocoverge-site/
    cd ../cocoverge-site && git add -A && git commit -m "Update site" && git push

`CNAME` holds the custom domain. `.nojekyll` disables Jekyll processing.
