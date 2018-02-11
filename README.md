# Dome360
A system for UE4 that outputs 360 or 180 video. 360 videos are output using equirectangular projection, 180 videos are output using fulldome projection (great for planetariums).

## How to use it
1. Drop the TextureCubeExporter into any scene.
2. Turn on "Use Fixed Frame Rate" in your Project Settings.
3. Play your level to begin the export process. The exporter will save out an image sequence of .hdr files.
4. Bring this sequence into a program like Adobe After Effects to render out to a video.
5. To make your 360 videos play properly on YouTube (or other platforms), use a program like Google's [Spatial Metadata Injector](https://github.com/google/spatial-media/releases).

## Settings
Select the TextureCubeExporter. In the details panel, you can change the following settings:
1. **File Path** - The location to save the output to.
2. **Clip Name** - The filename to use when exporting. Don't add an filetype extension; .hdr will be added automatically.
3. **Export Images** - Whether or not to export images when the scene plays.
4. **Preview Plane** - This allows you to choose a plane in the scene to preview the output. Very helpful!
5. **Width** - The width (in pixels) of the output.
6. **Height** - The height (in pixels) of the output.
7. **Dome Projection** - This toggles between equirectangular and fulldome projection.
8. **Dome Overlay Alpha** - This shows a helpful overlay when in fulldome projection mode.
