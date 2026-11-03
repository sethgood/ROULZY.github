ROULZY GALAXY - Gamepad Viewer skin (PS5 / DualSense)
=====================================================

1) Upload EVERY file in this folder to your GitHub repo (sethgood/ROULZY.github),
   replacing the old skin.css. Turn on Settings > Pages (branch: main, / root).
   Check that this opens and shows CSS text:
     https://sethgood.github.io/ROULZY.github/skin.css

2) YOUR GAMEPAD VIEWER LINK:
     https://gamepadviewer.com/?p=1&css=https://sethgood.github.io/ROULZY.github/skin.css

3) OBS: Sources > + > Browser > paste that link as the URL.
   Width 1049, Height 846. Leave Custom CSS empty.
   Plug the controller in, press a button, and it should light up.
   If OBS shows an old look: Browser Source > Refresh cache of current page.

Alternative (if the link doesn't work): use the plain Xbox skin link
   https://gamepadviewer.com/?p=1&s=1
and put this single line in OBS Custom CSS:
   @import url("https://sethgood.github.io/ROULZY.github/skin.css");

Based on CrazyGrape's DualSense skin layout (CC BY 3.0 US).
PlayStation / DualSense designs belong to Sony.
