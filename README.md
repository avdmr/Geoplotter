Python Scripts for Coloring Countries on a World Map Using a TXT List. Outputs an interactive map and PNG file

Usage:
- Download or fetch a new GeoJSON file using the fetch script, download and convert the (cultural) admin countries map from Natural Earth and convert to geojosn (https://www.naturalearthdata.com/downloads/), or use the provided GeoJSON files.
- Rewind the fetched files using the rewind script. (This addresses a known glitch in Plotly.)
- Use the geoplotter script to generate the colored map.


geoplotter Script Instructions
1. Place the script in a folder of your choice.
2. Create a folder named source inside this folder.
3. Inside the source folder, create another folder named geojson, and place the provided or fetched (and rewound) GeoJSON files there.
4. Create country lists (in ISO 2-letter or ISO 3-letter format, or a mix) inside the source folder. Name each file after the color you want to assign to the listed countries (e.g., red.txt).
5. The first line of each TXT file should be in the format:
   label: "<name of label>"
6. Optionally, create an ignore.txt file containing countries or areas that should not be colored. This is especially useful for ignoring overseas territories by adding their ISO codes to this file.

Example Files
red.txt
label: "apples"
USA
DK
VZ

green.txt
label: "potato"
TR
VU
EH

ignore.txt
GF
