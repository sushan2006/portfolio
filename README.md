# Sushan Reddy Portfolio

A single-page site. No build step.

## Run it
Open `index.html` in a browser. It works offline: the 3D library is in `vendor/three.min.js`
(three.js r128). Fonts (Geist) load from Google Fonts when you are online and fall back to
system fonts when you are not.

## Files
- `index.html`: everything (markup, styles, script)
- `vendor/three.min.js`: three.js r128
- `favicon.svg`, `favicon-32.png`, `favicon.ico`, `apple-touch-icon.png`: the keycap logo for browser tabs and phone home screens
- `og.png`: the preview image shown when the link is shared

## Edit your details
Near the top of the script in `index.html`:

```js
var CONTACT={email:"sushan.vaka@gmail.com",linkedin:"",resume:""};
```

Fill in `linkedin` and `resume` with full URLs. Empty values stay hidden.

Other content lives in the same script:
- `SECTIONS`: the six page keys and what the monitor shows for each
- `PROJ`: the six projects (key label, page text, facts)
- `INFO`: the six information keys (Education, Experience, Research, Stack, Hardware, Interests)

Page text for About, Process, What I do and Explore is plain HTML in the `<section class="page">` blocks.

## Pages
Each page has its own link through the hash: `#about`, `#projects`, `#process`, `#what-i-do`,
`#explore`, `#contact`, and one per project such as `#stockpro-ai`.

## Put it online (Vercel)
```powershell
npm i -g vercel
cd C:\Users\susha\Desktop\portfolio
vercel --prod
```
When it asks for the project name, type `portfolio-sushan`. If that name is free, the site
is served at `portfolio-sushan.vercel.app`. No build settings are needed.
