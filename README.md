FastPaint V.2.76 - KEYS, MOUSE AND FUNCTIONS
============================================
A Deluxe Paint style drawing program for the Atari STE (low resolution).
Developed in STOS BASIC + Extensions Missinglink, Control.
Includes assembly routines for increased speed.
Utilizes the STe Blitter and STe colors.
Converts BMP, PNG, IFF, GIF and other file formats.

START AND FILES
---------------
The program is FSTPAINT.BAS (compiled: FSTPAINT.TOS). The folder DATA must be
next to it and holds everything the program needs: ZOOM, VIEW, CLIP, KONV, FORM,
TEXT, BANK, DIALOG and DITHER.BIN, GRAFIKC.MBK, STOS8.FNT, the fonts in DATA\FONT
and this file. Settings are saved in DATA\FSTPAINT.INF.
FastPaint looks for DATA in the drive and folder it is started from, otherwise in


MOUSE
-----
Left button          Draws with the foreground colour (FG) using the current tool.
Right button         Draws with the background colour (BG).
Click a colour       Left = choose FG, right = choose BG (panel on the right).
                     If you have a clip as brush, the brush is drawn in one colour (FG).
Click an icon        Chooses a tool (see TOOLS below).
Pointer              An arrow over the panel and the brush chooser,
                     a cross in the picture. With the brush tool the
                     chosen brush is shown in the FG colour where it draws
                     (cross in zoom mode and when choosing a stencil colour).

GENERAL
-------
H                    Help screen with the most important keys.
Esc                  Cancels: curve, cutting, the menus, the brush chooser
                     and stencil choosing.
U                    Undo / redo (switches between the last and previous state).
                     Each window has its own undo.
F10                  Side panel off/on (the picture becomes 320 wide).
Space                The menus (see MENUS).
Arrow keys           Scroll big pictures: 16 pixels in x, 8 lines in y.
                     In zoom mode they move the magnified area.
Shift + arrow        Moves the pointer exactly 1 pixel (brush, clip or text follow).
                     In zoom mode: moves the zoom 1 pixel.
,  (comma)           Picks the colour under the pointer as FG.
+  -                 Brush size 1-15 (brush tool).
                     In zoom mode and with the zoom tool: magnification 2-4-8.

ZOOM
----
M                    Zoom on/off, centred at the pointer.
                     Left part = normal view, right part = magnified.
2  4  8              Chooses the magnification directly.
Zoom tool            An XOR box shows the area that will be magnified.
                     Left click = zoom, right click = change size 2-4-8,
                     + - = bigger/smaller box. Saved in FSTPAINT.INF.
All tools work in zoom mode, both in the magnified part and in the small
normal view. Shapes are drawn into the picture while you drag, so you see
exactly which pixels are coloured. Freehand cutting becomes a box in zoom mode.

BRUSH CHOOSER
-------------
Right click on       The brush chooser opens left of the panel:
the brush icon       round brushes 1-15 at the top, square brushes 1-15 below.
Left click           Chooses the brush (shown light). The choice stays.
Right click / Esc    Closes the brush chooser.
                     The panel works while the chooser is open. Choosing another
                     tool closes it. You cannot draw while it is open.
                     The stencil only works with square brushes.

CLIP AND BRUSH
--------------
Clip tool            Drag a box (or freehand) around what you want to cut out.
                     Right click on the clip icon = box / freehand.
                     Cut with the right button = transparent (BG colour removed).
C                    Gets the last clip back as brush (with its own colours).
.  (full stop)       Drops the brush (back to normal drawing).
Click a colour       The brush is drawn in that colour. C = its own colours again.
                     A clip is also kept in its own store (max 48 kB), used by
                     Fill: clip in the text dialog and by Reshape brush.

FILL
----
Fill tool            Fills the area with FG (right button = BG).
F                    Fill mode: colour / clip pattern / gradient. Same as right
                     click on the fill icon (the teapot changes look).
                     The pattern is laid from the picture's 0,0 so areas match.
                     Without a clip it fills with colour.
Right click on the filled box, filled circle or filled ellipse icon also switches
the fill mode for those shapes.

GRADIENT WINDOW
---------------
Choose the fill tool, F until gradient is chosen, then right click on the fill icon.
  From / To    start and end colour (left/right click in the colour row)
  Up / Down    which way through the palette the colours go
  Linear / Circle   Circle = From colour in the middle, To colour at the edge
                    (with the bucket: the middle is where you click)
  Angle        direction 0-359 degrees (- +, click the number and type, or click the dial)
  Pattern      Checker, Fine, Dots, Lines, Noise
  Width        1-100 %: how much of the area the transition takes
  Blend        1-100 %: how smoothly the colours mix (low = clear bands)
A sample is shown. Right click on - + = steps of 10. Used by fill, filled shapes
and text, and saved in FSTPAINT.INF.

GRID
----
G                    Grid on/off. The pointer snaps to the grid points.
R                    Grid setup: width, height, start X, start Y,
                     visible yes/no (dots that show the grid).
                     Left/right click = steps of 1/8.
                     OK/Return = keep, Cancel/Esc = as before.

STENCIL
-------
E                    Stencil on: pick the colour under the pointer. The pen and
                     the shapes then draw ONLY on top of that colour.
                     E again = off. A small mark in the colour box shows it is on.
                     (Not used by fill and clip brushes.)

MIRROR
------
V                    Mirror off / X (left-right) / Y (up-down) / both (four copies).
                     Everything drawn is mirrored around the middle of the picture:
                     freehand, brushes (clips are drawn flipped), lines, boxes,
                     circles, ellipses, curves, spray and filled shapes.
                     The bucket fill is not mirrored.

TEXT
----
T                    The text dialog (also the T icon, or Clip > Text).
                     At the top: the text - type directly, Backspace deletes (max 60).
                     The list: the fonts with a sample. Click = choose, click the
                     chosen one again (or Return) = OK. Up/Down and arrow keys scroll.
                     Size 4-200, Width 10-800 %, Italic -100..100, Bold 0-15,
                     Spacing -20..40: left click = small step, right = big step.
                     Prop. = proportional (narrow letters take less space).
                     Fill: colour / clip / gradient / none (none = only the edge).
                     Edge 0-6 = outline around the letters, the box next to it is
                     the outline colour (left click next colour, right previous).
                     When you change something, a sample is shown in the list area.
                     OK = the text becomes the BRUSH: it follows the mouse, click =
                     put it in the picture. Everything you can do with a brush works:
                     the grid (G) snaps the handle, A reshape (e.g. an angle with
                     Rotate), X Y Z < > O, click a colour = one colour, save as .CLP.
                     The handle box (same as Clip > Handle): where the mouse holds
                     the text. Left click = next position, right = previous.
                     Esc = close without doing anything (settings are kept).
                     The fonts are in DATA\FONT: FONTER.LST, FONTPROV.MBK (samples)
                     and the .FNV files. A font is loaded when it is used.

WINDOWS (PICTURE 1-8)
---------------------
F1 - F8              Switches to picture 1-8. Each picture has its own size,
                     palette, scroll and undo. A new window gets the size and
                     palette of the picture you came from. The brush is shared.

PICTURES AND FILES
------------------
L                    Load picture: NEO, PI1, PE1, BIT, MBK, BMP, PNG, GIF, IFF/LBM.
                     BMP, PNG, GIF and IFF open the import dialog:
                       Size     As now (scaled into the picture) / Original (1:1) /
                                Custom (width and height, with or without proportions)
                       Colours  2 / 4 / 8 / 16 (1-4 bitplanes)
                       Quality  Fast / Dither / Colour+ / Best
                       Palette  Calc (worked out) / Current (your palette) /
                                Picture (if it has at most 16 colours)
                     Other MBK banks (Missing Link bobs and joeys, CBK1/CJY1,
                     STOS sprites, packed STOS pictures) open a dialog:
                       Direction  Rows / Columns
                       Spacing    0-16 (images are placed in 16-pixel steps in x)
                       No room    Bigger picture (max 4096 x 4000) / Only those that fit
                       Palette    Bank / Adapt (nearest colour in your palette) / As is
S                    Save picture. The extension chooses the format:
                     320x200 16 colours: NEO PI1 PE1 MBK.
                     Other sizes: PE1 (4 bitplanes), BIT (1-3), MBK.
                     Without an extension .PI1 is added (PE1/BIT for other sizes).
K                    New picture (clears the picture).
B                    Picture size: width (steps of 16), height, bitplanes 1-4,
                     shows memory and file size.
I                    Saves all settings in DATA\FSTPAINT.INF (no message).
Q                    Quit (Y/N). The settings are saved in FSTPAINT.INF.

THE FILE SELECTOR
-----------------
Loading and saving use the CLFILE file selector (grey, with its own palette).
Double click = open folder / choose file. Click a column title = sort.
Right click = menu (rename, delete, mark/move, new folder, show all files).
The box next to the drive button shows the file filter: click to choose filters.
When SAVING: just type a name (a letter or digit starts the name field at the
bottom), or click in the name field to edit the name of the marked file.
Return/OK = save, Esc in the name field = back to the list. OK on a file in the
list overwrites it. Esc / Cancel = cancel.

PALETTE
-------
P                    The palette editor. Also right click on the FG/BG box in the panel.
                     R G B 0-15: - + (hold = count) or drag the slider.
                     Big box = the colour, all colours to the right (click = choose).
                     < > change colour. Save PAL = 32 bytes (STE format, as in NEO/PI1).
                     Load PAL takes a .PAL or the palette of a NEO/PI1.
                     Copy: click the colour to copy from, then the colour to copy to.
                     Swap: two colours change place in the palette (picture unchanged).
                     Merge: like Swap, but the pixels change too, so the picture looks
                     the same (good for sorting the palette).
                     Spread: click the first and last colour, the colours between
                     become an even transition.
                     Repl: click the colour to remove, then the colour it becomes
                     (only the picture changes).
                     Planes 1 2 3 4: which bitplanes everything you draw changes
                     (light = on). Other planes are left alone.
                     The status line shows "Copy from" etc. Right click or Esc cancels.
                     OK / Return = keep, CANCEL / Esc = the palette as before
                     (also the picture after Merge/Repl).

MENUS (SPACE)
-------------
Space gives a white menu bar at the top: File Fill Clip Options Window.
Move the pointer over a title to open the menu, click a line to choose it.
Click outside, space or Esc closes. A tick = on, a grey line = not possible now.
File     Load picture (L), Insert picture, Save picture (S), Load clip, Save clip,
         New picture (K), Picture size (B), Save settings (I), Help (H), Quit (Q).
Fill     Colour / Clip pattern / Gradient (as F), Gradient setup.
Clip     Last clip as brush (C), Drop brush (.), Reshape brush (A), Flip X / Flip Y,
         Rotate 90, Original (X Y Z O), Freehand cut, Cut inside grid (cut without
         the last grid line), Handle (left click next position, right previous),
         Text (T).
         Handle: where the mouse holds the brush/clip/text (top left ... centre ...
         bottom right). With the grid (G) that point snaps to the grid.
Options  Grid (G), Grid visible, Grid setup (R), Palette (P), Stencil (E: then pick
         the colour in the picture or the panel), Mirror off / X / Y / X+Y (V),
         Zoom (M), Side panel (F10).
Window   Picture 1-8 (F1-F8). A tick = the picture you are in, a dot = it exists.

TOOLS (THE PANEL, FROM THE TOP, LEFT/RIGHT)
-------------------------------------------
Freehand       | Brush (size with + -, right click = brush chooser)
Line           | Spray (right click = spray setup)
Box            | Filled box
Circle         | Filled circle
Ellipse        | Filled ellipse
Fill (teapot)  | Zoom
Undo           | Text (T)
Curve          | Clip
Curve: drag a line, release, move the pointer to bend it (the curve goes through
the pointer), right button fixes it, Esc cancels.
Freehand and brush painting is fast: no pointer is shown while the button is down.

SPRAY SETUP
-----------
Right click on the spray icon.
  Size     the radius of the spray, 1-24 pixels
  Speed    dots per frame, 1-40
  Colour   Pen (the pen colour) / FG..BG (random among the colours between the
           foreground and background colour in the palette) / Random (all colours)
Right click on - + changes by 5. A circle and a sample of the spray are shown to
the right. OK/Return keeps, Cancel/Esc undoes. Saved in FSTPAINT.INF.

RESHAPE BRUSH (A)
-----------------
Works when you have a brush (clip or text). The brush is always made from the
original cut-out, so it does not get blurred by many changes.
A                    The reshape dialog at the bottom, with a preview of the brush
                     above it (reshaped when you release the button). Also right
                     click on the clip icon, or Clip > Reshape brush.
  Row 1  Dither: Off / Ordered (pattern) / Diffuse (error diffusion), right click
         backwards, and the strength - + (5 %, right click 25 %; click the number
         to type it). The colours of the brush are mixed with their neighbours
         (1-25 % = 3x3 pixels, up to 9x9 at 76-100 %) and dithered to the
         picture's palette, so the transitions between colours become smoother.
         Takes about 1 second for a 64x64 brush. Off removes it again.
  Row 2  Width - + / Height - + (left click 1, right 10, max 640 x 400),
         lock = keep proportions, ring = round, 1:1 = size of the cut-out,
         Clip/Text = what is reshaped: the clip from the store or the text.
  Row 3  Flat / Globe / Fisheye with the amount - +, turn 0/90/180/270 (the F
         symbols), flip X / Y, rotate - + (left 1 degree, right 15).
  Row 4  OK, Original (as cut out), Cancel, and the size of the result.
Click a number = type it. Hold the pointer still over a button for 1 second
to see a short help text.
X / Y                Flip left-right / up-down
Z                    Turn 90 degrees clockwise
< >                  Rotate 15 degrees anticlockwise / clockwise
O                    The brush as cut out again
Outside the globe and the corners when rotating become transparent.

FSTPAINT.INF (IN DATA)
----------------------
Saved with I and at Q. Read at start. Holds the grid, fill mode, zoom, brush
(size and shape), panel, FG/BG, clip mode, menu height, picture size, palette,
the gradient and the spray settings.

HISTORY (SHORT)
---------------
V.2.00  Reshape brush and import (BMP, PNG, GIF, IFF).
V.2.10  All tools in zoom mode.
V.2.30  CLFILE file selector with filters.
V.2.36  Text tool. Stencil moved to E.
V.2.41  New palette editor (Copy, Swap, Spread, Merge, Repl, Save/Load PAL).
V.2.44  Load other MBK banks (bobs, joeys, sprites, packed pictures).
V.2.47  Mirror (V) and gradient fill. V.2.48 bitplanes in the palette.
V.2.52  Gradient window. V.2.59 circular gradient.
V.2.54  Menus on the space bar.
V.2.62  Everything in the program in English.
V.2.64  Fast painting with freehand and brush.
V.2.66  Shift + arrow = 1 pixel.
V.2.67  Outline (Edge) on text.
V.2.68  Compact reshape dialog with preview.
V.2.71  Clip store, Clip/Text in the reshape dialog.
V.2.72  Saving with the CLFILE file selector. Dither in the reshape dialog.
V.2.73  Title picture. The program is called FastPaint.
V.2.74  Help texts in the reshape dialog. Cancel in Grid setup.
V.2.75  Spray setup.
V.2.76  FSTPAINT.BAS with all its files in the folder DATA.
