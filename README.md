# Coloring

Miscellaneous tools for colormaps or otherwise dealing with color graphics.

## huecmaps

A set of seven carefully matched perceptually uniform sequential
colormaps.  These are tinted gray scales, designed particularly for
displaying multiple data sets (say density and temperature) in side
by side filled mesh plots, or to distinuguish several adjacent
materials when plotting a single quantity (say density of fuel and
ablator).  The seven maps, correspond to RGB and CMYK, called (in that
order) red, green, blue, cyan, purple, gold, and gray.

The (gold, blue, gray) set have nearly identical appearance to normal
and colorblind viewers.  The (blue, gray, red) set are close to the
hues in the diverging coolwarm colormap designed by Kenneth Moreland,
and are also easily distinguished by colorblind viewers.  Other
combinations are less colorblind-friendly.

All the maps are arranged from dark to light.  You can append "_r" to
the name to get the same map reversed (from light to dark).  You can
also append any pair of names to produce a diverging colormap, for
example "blue_red" goes from dark blue to light blue, switches to
light red and continues to dark red (very similar to coolwarm).  If
you want to go from light to dark to light, connect the map names with
"_r_", like "blue_r_red".  (Altogether 14 sequential and 84 diverging
colormap names are defined.)

The module defines a hueset object, which changes the current palette.
For example, hueset.gold changes the current palette to gold.  There
is also a hue object, which is the same as hueset except that it returns
the palette as a matplotlib colormap.

Here are the basic sequential color maps:

![huecmaps sequential maps](/huecmaps.png)
