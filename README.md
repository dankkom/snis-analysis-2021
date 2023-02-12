# SNIS Analysis 2021

Create GIF

```
ffmpeg -framerate 1 -pattern_type glob -i 'plots/maps/*.png' -vf "fps=10,scale=500:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 test.gif
```
