# Subs4Vita
TTML->M4T subtitle converter, mainly designed for PS Vita.
Converts standard TTML timed text XML into an M4T (TTML inside the ISOBMFF container).

# Configuration
Subs4Vita supports basic custom configuration which can be used to uniformly apply additional attributes to all styles and layouts when converting to M4T.
Configuration file must be named ``config.xml`` and placed together with ``s4v.exe``.
Configuration attributes will override original attributes from TTML, if present.
Supported configuration elements:
- styling
- layout

Example configuration:
```
<?xml version="1.0" encoding="UTF-8"?>
<tt>
<head>
  <styling tts:fontFamily="monospace"/>
  <layout tts:backgroundColor="transparent" tts:showBackground="whenActive"/>
</head>
</tt>
```

# Usage on PS Vita
0. Recommended: use together with the VideoDebug plugin.
1. Convert your subtitles to TTML. You can use [SubtitleEdit](https://github.com/SubtitleEdit/subtitleedit) with **Timed Text IMSC 1.1 (.xml)** preset.
2. Convert TTML to M4T. You can either drag and drop TTML files onto the s4v.exe or use command line: ``s4v example1.ttml example2.ttml``. Output M4T files will be created in the same folder as input.
3. Copy your M4T files to the PS Vita. M4T files must be in the same folder as video file and must have the same name.
4. Videos app will recognize subtitles automatically. You need to enable closed captions in the accessibility settings and click the "CC" button in the video player control panel.

Note that the extent of the TTML features supported on Vita is unknown, some styling may not work.
