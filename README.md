**SFCalcSheet** – Science fiction calculation spreadsheet


### Summary ###

This is a [LibreOffice Calc](https://www.libreoffice.org) spreadsheet for performing various science fiction and astronomy related calculations. The aim is to cover all common math problems in SF while keeping it simple for the user. The spreadsheet can assist with worldbuilding in science fiction and fantasy, or be used as an aid in amateur astronomy.

Apart from LibreOffice, SFCalcSheet works very nicely in a number of additional office suites including [Google Sheets](https://docs.google.com/spreadsheets), [Excel Online](https://www.office.com/launch/excel) and [Collabora Office](https://www.collaboraoffice.com/).

To get started you can check out the [releases page](https://github.com/lortordermur/sfcalcsheet/releases) or [browse the formulas](https://github.com/lortordermur/sfcalcsheet/wiki/Formulas) that are used in the spreadsheet. If you would like to share informal feedback or constructive criticism, there is an [official Reddit thread](https://www.reddit.com/r/worldbuilding/comments/iodfba/sfcalcsheet_science_fiction_calculation) as well.


### Included calculators and converters ###

* **Constants**: Collection of physical constants used in the spreadsheet’s internals.
* **Conversion**: Unit conversion.
  * Light years <-> parsec
  * km <-> AU
  * m/s <-> km/h
  * Temperature
  * Length (SI <-> USCS)
  * Area (SI <-> USCS)
  * Volume (SI <-> USCS)
  * Mass/weight (SI <-> USCS)
  * Simple calculator
* **Star**: Star related calculators.
  * Magnitude <-> luminosity
  * Magnitude/distance
  * Luminosity difference
  * Star color
  * Star properties
  * Binary orbit
* **Planet**: Planet calculators.
  * Mass converter
  * Physical properties
  * Orbital properties
  * Tidal forces
  * Planetary habitability
  * Population density
  * City area
* **Satellite**: Calculators pertaining to natural satellites, i.e. moons.
  * Satellite appearance
  * Satellite orbit
* **Compact**: Compact object calculators.
  * Schwarzschild black hole properties
* **Impact**: Impact calculators.
  * Impact and crater
  * Neutron matter explosion
  * Bomb blast
* **Life**: Calculators related to living beings.
  * Creature body weight
  * Vegetation color
* **Structure**: Calculators for large structures.
  * Structure properties and resources
* **Vehicle**: Vehicle calculators.
  * Vehicle mass and personnel
* **Travel**: Travel calculators.
  * FTL factor
  * FTL travel time
  * Time dilation
  * Uniform acceleration
  * Terrestrial travel time


### Write protection ###

To avoid overwriting the default values by an accidental save, the spreadsheet file can be write protected in Unix-like environments using `chmod 444 sfcalcsheet.ods`. These permissions allow for the file to be opened for editing (you might get an additional prompt for this) but it cannot be saved back to the same file. You can make the file writable again with `chmod 664 sfcalcsheet.ods`.


### Caveats ###

SFCalcSheet attempts to keep algebraic complexity on a manageable level for the sake of maintainability. The following formulas are simplistic approximations and should not be used for work requiring scientific accuracy:

* Star radius
* Star temperature
* Star habitable zone
* Roche limit
* Greenhouse effect part of planetary temperature
* Impact crater size
* Bomb blast fireball radius
* Vegetation color
* Vehicle mass


### Frequently asked questions ###

**Does it really work in office suites other than LibreOffice?**

Yes, but in several cases only with serious flaws that cannot be fixed in the spreadsheet. SFCalcSheet uses some pretty fancy OpenDocument functions and cell styles, and therefore cannot be guaranteed to fully function in every office software. Apart from LibreOffice it has been tested in the following office suites featuring OpenDocument support:

* **Desktop software**

  * **Collabora Office**: Based on current LibreOffice. ***Completely functional*** without visual glitches.
  * **SoftMaker Office**: Well-functioning but calculator headings don’t show, as well as some background colors in random places.
  * **SoftMaker FreeOffice**: Outdated OpenDocument support, only partly functional.

* **Web applications**

  * **Google Sheets**: ***Completely functional*** after post-v0.09 fixes. Visual glitches with framed cells.
  * **Microsoft 365**/**Excel Online**: ***Near-completely functional*** after post-v0.10 fixes. The only broken parts are the display of star color temperature and the height of word-wrapped cells.
  * **Zoho sheet**: Mostly functional but calculator headings don’t show, and calculators using the IFS function (such as “Simple calculator” and “Structure properties and resources”) don’t work.

* **Android apps**

  * **Collabora Office**: Same engine as the desktop software, ***completely functional***.
  * **Google Sheets**: Same engine as the web application, ***completely functional***.
  * **Excel/Microsoft Office**: Outdated OpenDocument support, only partly functional.
  * **AndrOpen Office**: Outdated OpenDocument support, only partly functional.
  * **Zoho Sheet**: Same engine and glitches as the web application.
  * **OpenDocument Reader**: All text displayed white on black, editing non-functional.
  * **ONLYOFFICE documents**: Input text and most result text displayed in black, only partly functional.

Alas, many of the remaining glitches cannot be fixed without breaking SFCalcSheet in LibreOffice, because oftentimes OpenDocument support is outdated or incomplete.

**Where can I see the equations?**

Most of the math is (invisibly) performed in the cells right of the calculator boxes. If you move the selection to those you can see the formula in the input line at the top of the window. However, the wiki has it conveniently [all on one page](https://github.com/lortordermur/sfcalcsheet/wiki/Formulas).

**What are those 12.34E+56 numbers about?**

It is scientific exponential notation for very large and very small numbers. “E” is a shorthand for “ten to the power of”. Hence, 12.34E+56 is identical to 12.34 ✕ 10⁵⁶, and 12.34E-56 is identical to 12.34 ✕ 10⁻⁵⁶.

**I am tired of typing sizable numbers with lots of zeros.**

Fortunately, the aforementioned exponential notation is available in every numerical input field in SFCalcSheet. If you need to do some preparatory math before keying in the values, use the “Simple Calculator” on the Conversion sheet or type your calculation into [Google](https://www.google.com) or [Wolfram Alpha](https://www.wolframalpha.com).

**I miss a specific calculator or feature.**

Great, and this can be helped! Just file an issue on [sfcalcsheet’s issue tracker](https://github.com/lortordermur/sfcalcsheet/issues) and I will look into it.

**I cannot edit cell styles. The dialog simply does not open.**

To fix this you must unprotect all sheets. You can do so by selecting all tabs using shift-click and selecting `Tools->Protect Sheet` from the main menu.

**I would like to see the hidden interim calculations.**

This can be easily done by editing a cell style. Bring up the styles sidebar using the F11 key and right-click on the “InterimResult” style. Choose to edit, and on the font effects tab set the text color to anything other than black.

**Some cells containing large results are too narrow for their content. What can I do?**

Unlock the current sheet using `Tools->Protect Sheet` and then use the handles on the column bar to adjust the width.


### How you can support the project ###

There are a couple of ways you can participate and help:

* Leave some feedback, praise or anecdotes [on Reddit](https://www.reddit.com/r/worldbuilding/comments/iodfba/sfcalcsheet_science_fiction_calculation).
* [Star](https://github.com/lortordermur/sfcalcsheet/stargazers) SFCalcSheet on GitHub.
* [File an issue](https://github.com/lortordermur/sfcalcsheet/issues) on GitHub for a long-standing quirk or wanted feature.
* Test and debug SFCalcSheet on various office suites. 99% of this is work on cell styles and determining whether a software does not support certain functions, conditional formattings or text/frame features. If you manage to fix a glitch and it does not break SFCalcSheet in LibreOffice and other office suites, please post step by step instructions for it on the Reddit thread.
