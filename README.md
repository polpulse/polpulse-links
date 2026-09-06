# PolPulse — GitHub Pages website

This is a static website. No build command, package installation, database, API key or application server is needed.

## Publish

Keep these files together in the folder that GitHub Pages publishes:

- index.html
- assets/ (the entire folder)
- followers.json
- og.jpg
- CNAME (retains links.polpulse.co.uk)

Upload the contents of this folder, not an extra enclosing folder. Preserve the repository's existing Pages branch and folder settings. All page assets use relative paths, so the layout also works on a GitHub Pages project URL.

CNAME and the canonical/social metadata refer to the existing custom domain. Change those only if you move to a different domain.

## Update follower figures

Edit followers.json. Counts can be numbers or strings such as "17.4k". Use YYYY-MM-DD for updated. The page adds the available platform figures and notes that audiences may overlap. These are manually maintained figures, not live social API data.

If the file is missing or invalid, the social links remain usable and the community strip shows the number of official channels instead.

## Design and performance

The CSS and small enhancement script are in index.html. The font and compressed images are local to this folder; mobile browsers receive a smaller Westminster image. There are no frameworks, icon libraries, video embeds or external font services. Links and navigation work without JavaScript. Reduced-motion preferences are respected.

The existing GoatCounter analytics loads asynchronously after the main page load. It is disabled on localhost and file previews. Clipboard access requires HTTPS or localhost; email links work regardless.

Double-clicking index.html previews the design. To preview follower loading, serve the folder with any static HTTP server. GitHub Pages serves followers.json normally.
