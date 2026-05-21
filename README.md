One Puck Shot Trainer

The One Puck Shot Trainer is a simple air hockey learning and coaching tool built from an idea by Sammy and Chelsea.

It started as a shot trainer with one puck in the center of the screen that changes color, text, and explanation based on the selected shot. The app has now grown into a local graphic viewer and coaching whiteboard for teaching air hockey shots, table positioning, puck paths, defense concepts, and beginner fundamentals.

Live app:

https://petesimple.github.io/oneshot/

Current Build

Version: v6.7
Codename: Nice

What It Does

The app lets players and coaches choose from a local library of air hockey graphics, including motion shot diagrams, table graphics, table reference images, and coaching backgrounds.

Users can view any selected graphic full screen or open it in whiteboard mode.

Main Features

Single Graphic Selector

The app uses one simple dropdown for all available graphics.

Motion shots are highlighted at the top of the list with ⭐ MOTION.

Table graphics are listed underneath.

This keeps the app simple and avoids needing separate selectors for shots, tables, and whiteboard backgrounds.

Graphic Viewer

The View Graphic button opens the selected graphic in a clean full screen viewer.

This is useful for quickly showing a shot path, table layout, or reference image.

Whiteboard Mode

The Whiteboard button opens the selected graphic as a coaching board.

Coaches can draw directly on top of the selected graphic using the pen tool, eraser tool, color picker, brush size slider, clear button, and Save PNG button.

Movable Coaching Objects

Whiteboard mode includes movable coaching tools: Mallet, Red puck, Yellow puck, and Move tool.

These can be placed on the board and dragged around to demonstrate puck position, defensive coverage, shot setup, player movement, or table awareness.

Save PNG

Whiteboard drawings can be saved as a PNG file.

The saved image includes the selected background graphic, placed pucks and mallets, and any drawing marks or coaching notes.

Folder Structure

The app expects graphics to be stored locally in the repository.

Main Graphics Folder

graphics/

Used for table graphics, pucks, mallets, and reference images.

Examples:

graphics/Mallet.png
graphics/Red-Puck.png
graphics/Yellow-Puck.png
graphics/tablegraphicupdown.png
graphics/tablegraphicleftright.png
graphics/photonupdown.png
graphics/photonleftright.png

Shot Graphics Folder

graphics/shots/

Used for motion shot graphics and animated GIFs.

Examples:

graphics/shots/motioncross.gif
graphics/shots/motioncrossLR.gif
graphics/shots/motionRWU.gif
graphics/shots/motionRWO.gif
graphics/shots/motionLWU.gif
graphics/shots/motionLWO.gif
graphics/shots/DEFstraights.gif
graphics/shots/DEFwalls.gif

Motion Shot Categories

The current graphics library includes motion examples for straight shot defense, wall shot defense, cross shots, reverse crosses, cut shots, right wall under and over, left wall under and over, double banks, triple banks, and turkey shots.

Table Graphics

The app supports multiple table graphics and table styles, including generic table graphics, Dynamo table graphics, Brunswick table graphics, Gold Standard Games graphics, Photon graphics, FaceOff table graphics, reference photos, and wallpaper backgrounds.

How To Add More Graphics

To add a new graphic, upload the image file into either graphics/ or graphics/shots/.

Then add a new object to the GRAPHICS array in the JavaScript.

Example motion shot object:

{
type: “motion”,
label: “⭐ MOTION • New Shot Name”,
file: “graphics/shots/new-shot.gif”,
family: “Cross”,
name: “New Shot Name”,
note: “Short coaching explanation.”
}

Example table graphic object:

{
type: “table”,
label: “TABLE • New Table Graphic”,
file: “graphics/new-table.png”,
family: “Table”,
name: “New Table Graphic”,
note: “Plain table whiteboard background.”
}

Important File Note

GitHub Pages is case sensitive.

That means graphics/Mallet.png is not the same as graphics/mallet.png.

Make sure filenames in the code match the uploaded filenames exactly, including capitalization, spaces, and punctuation.

Suggested Use Cases

This app is useful for coaching new air hockey players, explaining shot names, teaching puck paths, showing defensive positioning, demonstrating wall shot coverage, drawing practice plans, teaching table awareness, and helping players understand setup, movement, and lane control.

Release Notes

v6.7

Codename: Nice

This build adds the new whiteboard coaching flow.

New in this version:

Local graphics support
One clean graphic selector
Motion shots highlighted at the top of the list
Full screen graphic viewer
Whiteboard drawing mode
Movable mallet tool
Movable red puck tool
Movable yellow puck tool
Move tool for repositioning objects
Save PNG export for coaching diagrams

This version turns One Puck Shot Trainer into both a shot learning tool and a practical air hockey coaching whiteboard.

Credits

Inspired by Sammy and Chelsea
Created by Pete
Built to help air hockey players learn, coach, and have fun
