# extension-template
Quickly start building a browser extension with React, TypeScript and webpack HMR!

# Overview
Easy template for getting started building extensions configured for React, TypeScript, and webpack hot reloading.

Currently tested and working with Chrome 

Note: HMR does not work for Content / Background scripts, you must restart browser to trigger Content / Background script updates

## Quick Install Guide:

1. Fork & clone this repo
`git clone https://github.com/[your-git-handle]/extension-template.git`

2. Install node modules
`npm i`

3. Start dev server & build dev bundle
`npm run dev`

## Install your extension in Chrome:

1. In Chrome, navigate to the URL `chrome://extensions/`

2. Enable `Developer mode` on the top-right of page

![image](https://github.com/dev-cameron/extension-template/assets/119974281/9cd1c8b0-659b-4627-bc1a-d94a826a71ab)

4. Click `Load unpacked` and navigate to the `/dev` bundle that was created, upload that folder

5. Enable your extension with the toggle button
   
![Alt text](image-3.png)

6. (Optional) pin your extension for easily toggling the main interface (`popup.html` in the dev bundle)
   
![Alt text](image-1.png)

8. Enjoy! Your extension should popup with **Hello, world!** when you toggle the icon
   
![Alt text](image-4.png)

## Developer notes:

To trigger HMR for your .tsx components, you need to toggle your extension's popup window after you save your changes. 

## Known issues:
- HMR currently not functional with Background and Content scripts, looking into how to implement.
