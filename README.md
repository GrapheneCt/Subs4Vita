# Subs4Vita
TTML->M4T subtitle converter, mainly designed for PS Vita.
Converts standard TTML timed text XML into an M4T (TTML inside the ISOBMFF container).

# Usage on PS Vita
0. Recommended: use together with the VideoDebug plugin.
1. Convert TTML to M4T. You can either drag and drop TTML files onto the s4v.exe or use command line: ``s4v example1.ttml example2.ttml``. Output M4T files will be created in the same folder as input.
3. Copy your M4T files to the PS Vita. M4T files must be in the same folder as video file and must have the same name.
4. Videos app will recognize subtitles automatically. You need to enable closed captions in the accessibility settings and click the "CC" button in the video player control panel.

Note that the extent of the TTML features supported on Vita is unknown, some styling may not work.
