# PCBee #

PCBee is a printed circuit board designed to look like a bumble bee.
It was designed using [PCBmodE](https://pcbmode.com).

## How to build ##

PCBmodE documentation is available on their website and is necessary for understanding the flow of the tool.
However the basic commands for compiling the board are included below:

To compile the board into an SVG, run `pcbmode -b pcbee -m`.

After making changes to the SVG in Inkscape, you can extract those changes with 
`pcbmode -b board --extract-from-svg` (or `-e` for short).

To build Gerber files to send out for fabrication, run `pcbmode -b pcbee --fab`.
Your Gerber files will be in `pcbee/build/production`.