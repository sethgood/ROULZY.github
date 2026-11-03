ROULZY GALAXY - Gamepad Viewer skin (PS5 / DualSense)
=====================================================

STEP 1 - Put the files on GitHub
  1. Sign in at github.com > New repository. Name it: roulzy-skin  (set it to Public).
  2. Click "uploading an existing file" and drag in EVERY file from this folder
     (skin.css, body.webp and all the .png files). Click Commit.
  3. Repository > Settings > Pages > Source: "Deploy from a branch",
     Branch: main, folder: / (root) > Save.
  4. Wait 1-2 minutes. Your skin file is then at:
        https://YOUR-USERNAME.github.io/roulzy-skin/skin.css
     Open that address in a browser - if you see CSS text, it's live.

STEP 2 - Set it up in OBS
  1. Go to gamepadviewer.com, pick the XBOX skin (or leave skin blank),
     plug your controller in over USB, press a button so it's detected,
     and generate your URL. Copy it.
  2. OBS > Sources > + > Browser. Paste that URL.
  3. Width: 807   Height: 651
  4. In "Custom CSS", DELETE everything and paste this one line
     (swap in your GitHub username):
        @import url("https://YOUR-USERNAME.github.io/roulzy-skin/skin.css");
  5. OK. Move sticks / press buttons to test.

If the @import line doesn't work: open skin.css, put your full GitHub
address in front of every file name inside url(...) , e.g.
   url(body.webp)  ->  url(https://YOUR-USERNAME.github.io/roulzy-skin/body.webp)
then paste the whole file into Custom CSS instead.

Files
  body.webp        animated galaxy controller (transparent background)
  stick.png        stick caps (normal + pressed)
  btn.png, dpad-*.png, create.png, options.png, bumper-*.png,
  trigger-*.png, touchpad.png, ps.png    glow shown when pressed
  body-static.png  still picture of the controller (backup, not used by the CSS)

Notes
  - Touchpad and PS button only light up if your setup passes them through
    to the browser (Steam Input / DS4Windows can help).
  - Based on the xbox-skin method of CrazyGrape's DualSense skin
    (CC BY 3.0 US). PlayStation / DualSense designs belong to Sony.
