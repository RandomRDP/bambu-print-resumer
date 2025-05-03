# bambu-print-resumer
Has your print failed? Do you wish you could resume it where it left off? Perhaps you've watched the [CNC Kitchen Video](https://www.youtube.com/watch?v=-wjE8eDiKWg) and still can't figure it out. Fear not, that's what this little tool is for.

# How it works
You must have python set up
Export your Gcode from bambu studio
Run the python script:
```bash
python ResumeBambuGcode.py
```
Follow the prompts (you'll need to measure the height of your print in millimeters)
It will output a new GCODE file
It's worthwhile opening the GCODE file in bambu studio to make sure it looks correct before printing
Save the new GCODE file to your micro SD card, put it directly into the bambu printer, and print!

# Issues
If the z-height isn't correctly calibrated, it might go to the wrong spot and run into your print. I have an idea to fix this (basically an option that allows you to home your z-axis in a safe area of the print bed).
