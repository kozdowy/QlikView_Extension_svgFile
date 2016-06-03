QlikView Extension svgFile
==========================

A simple extension to display an SVG file and use it with QlikView data. This has less features than svgMap extension but is probably more stable.

![QlikView Extension svgFile](screenshot.PNG)

![QlikView Extension svgFile](screenshot1.PNG)

Properties:
-----------

1. Section ID: Dimensions, SVG ID to link the data, colors and popup to the SVG element or path
2. Label: Expression for Region Label
3. Color Expression: Color code for section, use Color, RGB or HSL function
4. Popup contents: Shows text from expression as popup on hovering
5. Load SVG File: filename of the SVG file, should be copied into the extension folder
6: SVG Path Prefix: to generate unique SVG element or path IDs this prefix will be replaced by Object ID (from container DIV), use this as prefix for all element IDs (with inkscape or else)

Piece of advice:
----------------
SVG id's for elements or path' are case sensitive! Keep this into account to set up your dimension data. If not, SVG elements will probably not match with your data.
The labels should be mapped to the region by means of appending "-T" to the end of the region id

Changes Made:
-------------
Labels are now editable, and don't break the popups when hovering over the regions
Popup no longer has the ID at the very top by default
