# FuckYouTube
Block midroll ads on YouTube, without being detected.

## Installation
To install the FuckYouTube Chrome extension, follow the steps below:

1. Head to the [releases page](https://github.com/Mirrrek/fuck-you-tube/releases/latest) and download the latest release file `fuck-you-tube-<version>.zip`
2. Unzip the extension into a folder somewhere safe on your computer
3. Open up the extension manager by typing `chrome://extensions` into the search bar
4. Switch to developer mode by toggling the button at the top-right of the page
5. Click `Load unpacked` on the top-left of the page
6. Navigate into the folder you unzipped the extension into (it should contain a file `manifest.json`, though that might not show up in the file picker)
7. Hit `Select Folder` and a new extension called `FuckYouTube` should pop into existence
8. You're done! Make sure to reload any YouTube page open for the extension to kick in

## Development
Though this extension is currently dead simple, some updates and maintaining work might be necessary in the future. I'm open to push requests, so feel free to build on top of this.

1. Clone this repo
    ```
    git clone https://github.com/Mirrrek/fuck-you-tube.git
    ```
2. Make a new branch for your work
    ```
    git checkout -b <name-of-your-feature-or-fix>
    ```
3. Setup your environment  
   Assuming you have the following dependencies:
   - [Node.js](https://nodejs.org/)
   - npm (bundled with Node.js)
   ```
   npm i
   ```
4. Build the project (development)
   ```
   npm run dev
   ```
   This command will start webpack under watch mode, so saving a change to any source file will rebuild the extension automatically.  
   You can now add the `dist` folder as an extension to Chrome similarly as in the [installation steps](#installation).
5. Build the project (production)
   ```
   npm run build
   ```
   The extension files will be generated in the `dist` directory.

## Disclaimer
Blocking advertisements violates the [YouTube TOS](https://www.youtube.com/t/terms). This repository serves educational purposes only. I claim no responsibility in any misuse of the code provided.
