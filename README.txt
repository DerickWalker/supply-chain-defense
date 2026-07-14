Supply Chain Defense — Usage Guide
====================================

[supply-chain-defense.html]
Open it in any browser to play immediately. No installation needed.

[mobile-install folder]
To install this on mobile as an app (PWA), the folder needs to be hosted
on the web first:
1. Drag and drop this folder onto vercel.com/new (or run `npx vercel --prod`
   from inside it)
2. Open the resulting https link on your phone's browser
3. You'll be prompted to "Add to Home Screen" / "Install app" — do that
Opening index.html directly (locally) still runs the game fine, but the
install prompt itself only shows up once it's served over https.

[desktop-source folder]
Source for the Windows/Mac/Linux desktop app. A pre-built .exe isn't
included in this download to keep the file size small — Electron apps
bundle a full browser engine, so the compiled app is always ~70MB
regardless of how simple the game itself is, and compressing it further
doesn't help (it's already compressed internally).

To build it yourself, it only takes two commands. From inside this folder,
with Node.js installed:
  npm install
  npm run dist:win    (produces a Windows .exe in a new "dist" folder)
  npm run dist:mac    (Mac)
  npm run dist:linux  (Linux)

If you'd rather not build it yourself, ask and a pre-built .exe can be
provided as its own separate download instead.
