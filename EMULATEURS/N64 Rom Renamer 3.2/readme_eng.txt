# N64 Rom Renamer v3.2
#
# (c) 2000 by Einstein II.
# for more information and updates see http://www.emunews.de/renamer
# or email me: webmaster@emunews.de




Contens of this readme file:
----------------------------
   1.1   - What is this ?
   1.1.1 - Contents of the ZIP-file
   1.1.2 - Problems / Missing files
   1.2   - How many ROMs are recognized ?
   1.3   - Contact or what to do if a game is not recognized
   1.4   - What's new / Plans / Known bugs
   2.1   - Disclaimer

              -= * =-

1.1 - What is this ?
--------------------
This tool trys to find the country, the version and the full name of a ROM using the 
internal ROM-id, a CRC1-method if necessary and a database (ROMS.DAT). With this data
a filename is generated and you have the option to rename the ROM to this filename.

1.1.1 - Contents
----------------
n64romrenamer_eng.exe - english EXE-File
roms.dat              - Romdatabase
readme_eng.txt        - english Readme
COMCTL32.OCX and
COMDLG32.OCX          - ActiveX-Controls

1.1.2 - Problems / Missing files
--------------------------------
- The ROMS.DAT file should not be modified ! Any modification of this fileformat
  (blank lines, comments etc.) will cause program errors !

- The program needs the VB6-Runtimes and will ask for the MSVBVM60.DLL file if you
  don't have it. You can get it at http://www.emunews.de (click on N64 ROM Renamer).
  Simply download the VBRUN60.EXE and execute it - thats it.

1.2 - How many ROMs are recognized ?
------------------------------------
   1179 commercial games
     47 revisions, hacks and cracks via CRC1-Method
    139 demos and homebrewn games
   ----
   1365 N64 ROMs
   =============

1.3 - Contact or what to do if a game is not recognized
-------------------------------------------------------
Suggestions ? Errors ? Want to send me some money ?
Homepage: http://www.emunews.de
Email: webmaster@emunews.de

If you find a game that is not recognized by this program and you get the message
"Unknown ROM", then send me an email please so that this game can be recognized in
future versions. To really help me use the batchmode because a file named Unknown.log
will be created that contains all the necessary information about the ROM. It would be 
great if you email me this file.

1.4 - What's new / Plans / Known bugs
-------------------------------------

What's new ?
-----------------------------------------
| - 12. May 2000 v3.2 Sixth Release   - |
-----------------------------------------
    - Added many new signatures to ROMS.DAT -> all new games will be recognized
    - ROMS.DAT-Format changed -> higher recognition rate (should be near 100 % !)
    - The ROM-Size in MBit is displayed in single file mode
    - Fixed an error with the progressbar in batchmode (sometimes the bar didn't increase)
    - ROM-Images will now get the correct extensions: .v64 for Dr. V64 files, .z64 for
      Mr. Backup files and .n64 for the Fliprom format.
    - Statistics are displayed immediadtely in Batchmode
    - Sorting in batchmode enhanced:
      - renamed ROMs are moved to the subdir Renamed_N64_ROMs
      - unknown ROMs are moved to the subdir Unknown_ROMs
      - ROMs in a possibly unknown format and all other files are left untouched



-----------------------------------------
| - 18. March 2000 v3.1 Fivth Release - |
-----------------------------------------
    - added new signatures to ROMS.DAT -> higher recognition rate
    - Zero-Byte-File-Bug in batchmode fixed ;-)
    - improved the batchmode:
      - Duplicates now will be moved in a subdir called Duplicates
        (no more errormessages about duplicates !)
      - Unknown ROMs will be moved in a subdir called Unknown_ROMs
      - if there are unknown ROMs, a file called UNKNOWN.LOG is created that 
        contains all the necessary information to add this ROM to the next release.
        Please send this file to me (webmaster@emunews.de) if you got unknown ROMs !
    - Gamelistfeature: In batchmode you have the choice to let the ROM Renamer generate
      a detailed list of your games in HTML-format
    - Layout improved so the GUI is also in 800*600 mode full visible
    - new About-Dialog
    - Windowhandling bugfixed (in the last version the about- and the editorwindow could
      be "swallowed" by the main window)


-----------------------------------------
| - 12. March 2000 v3.0 Fourth Release - |
-----------------------------------------
    - Many internal changes - code new structured
    - Many bugfixes
    - roms.ini -> ROMS.DAT
    - Many new games to ROMS.DAT added, ROMS.DAT additional versions of existing
      games added  -> higher recognition rate
    - Clayfighter 63 1/3 caused an error becuase in the Jolietfilesystem it's not allowed
      to use / in the filenames - fixed
    - Toukon Road-Entries corrected - before Toukon Road was recognized as Tukon Road 2
    - Rally '99-Entries corrected - before Rally '99 was recognized as V-Rally '99
    - CRC1-Method improved to additional 59 games, hacks and revisions, now total 104
    - Countrycodes added: S = Spain (PAL), A = USA or Japan (NTSC)
    - Wordswapped ROMs are now recognized (Flipromformat)
    - CRC2 is displayed
    - Headereditor
    - new "About"-Dialog
    - Exit bug fixed (sometimes the program has remained in memory)


-----------------------------------------
| - 27. Jan 2000 v2.1 Third Release - |
-----------------------------------------
    - fixed a bug that caused a short flashing at the start (no real bug ;-)
    - bugfix in the CRC1-Method which sometimes reported some N64-ROMs as unknown
      (e.g. Pokemon Snap)
    - Zelda v1.1 is now recognized correctly and no longer as normal Zelda
      (via CRC1-Method)
    - ROMs with countrycode X are now correctly recognized as PAL-Australian
      (before unknown country)
    - improved the errorhandling routine - now clear an better errormessages
    - enhanced the CRC1-Method. Every ROM can now be recognized theoreticly, no
      more unidentificable ROMs !
    - internal CRC1-Database enhanced to 49 ROMs total
    - new "About"-Dialogue
    - Check at the start if the roms.ini is there


-----------------------------------------  
| - 14. Jan 2000 v2.0 Second Release - |
-----------------------------------------
    - Bugfix when reading the headerdata:
      Some N64 ROMs were not recognzized as N64 ROMs e.g.
       - Shadows of the Empire
       - Star Wars E1 POD Racer
       - NBA Hangtime
       - New Tetris
       - Quake 64
       - Cruisin USA
       - Doom 64
      This is now fixed.
    - Batchmode (yeah !)
    - UltraHLE-like filenames (spaces are replaced by _)
    - Statistics after batchmode
    - Correct name of the fileformat:
      Byteswapped = Dr. V64 Format, normal = Mr.Backup Z64 Format
    - CRC1-Method, this is good for recognizing roms that have the same internal name,
      Pokemon Snap Station is no longer recognized as Pokemon Snap
    - ROM-Database enhanced (422 ROMs are recognized)
      and different versions of the internal ROMnames were added so the recognitionrate is
      much higher


----------------------------------------
| - 3. Jan. 2000 v1.0 First Release - |
----------------------------------------
    - Filemode to rename single ROM-Images



For future versions, the following features are planned:
  - more Roms should be recognized ;-)
  - the batchmode should be more error tolerant (e.g. if two files have the same 
    filename)
  - ...more suggestions ?

Known Bugs:
  - 2 Blokes and an Armchair Demo is not recognized as N64ROM because of a wrong header

2.1 - Disclaimer
----------------
You will use this program at your own risk ! The author is in no way responsible for
any damage that this program may cause, directly or indirectly.


  ...and sorry for my bad english ;-)