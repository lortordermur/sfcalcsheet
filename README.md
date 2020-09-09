**SFCalcSheet** – Science fiction calculation spreadsheet for LibreOffice


### Summary ###

This is a [LibreOffice Calc](https://www.libreoffice.org) spreadsheet for performing various science fiction and astronomy related calculations. The aim is to cover all common math problems in SF while keeping it simple for the user. The spreadsheet can assist with world-building in science fiction and fantasy, or be used as an aid in amateur astronomy.

To get started you can check out the [releases page](https://github.com/lortordermur/sfcalcsheet/releases) or [browse the formulas](https://github.com/lortordermur/sfcalcsheet/wiki/Formulas) that are used in the spreadsheet.


### Included calculators and converters ###

* **Constants**: Collection of physical constants used in the spreadsheet's internals.
* **Conversion**: Unit conversion.
  * Light years <-> parsec
  * km <-> AU
  * m/s <-> km/h
  * Temperature
  * Length (SI <-> USCS)
  * Area (SI <-> USCS)
  * Volume (SI <-> USCS)
  * Mass/weight (SI <-> USCS)
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

To avoid overwriting the default values by an accidental save, the spreadsheet file can be write protected in Unix-like environments using `chmod 444 sfcalcsheet.ods`. These permissions allow for the file to be opened for editing (you might get an additional prompt for this) but it cannot be saved to the same file. You can make the file writable again with `chmod 664 sfcalcsheet.ods`.


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

**Does it work in office suites other than LibreOffice?**

Not without flaws so far. SFCalcSheet uses some pretty fancy OpenDocument features and formatting, and therefore cannot be guaranteed to fully function in every office software. Apart from LibreOffice it has been tested in the following:

* **Desktop software**

  * **Collabora Office**: Based on current LibreOffice. Both the Android and desktop versions work flawlessly and without visual glitches.
  * **SoftMaker Office**: Completely functional but calculator headings don’t show, as well as some background colors in random places.
  * **SoftMaker FreeOffice**: Outdated OpenDocument support, only partly functional.

* **Web applications**

  * **Google Sheets**: Completely functional after post-v0.09 fixes. Visual glitches with framed cells.
  * **Microsoft 365**/**Excel Online**: Near-completely functional after post-v0.10 fixes. The only broken parts are the display of star color temperature and the height of word-wrapped cells.

* **Android apps**

  * **Collabora Office**: Same engine as the desktop software, completely functional.
  * **Google Sheets**: Same engine as the web application, completely functional.
  * **Excel**: Outdated OpenDocument support, only partly functional.
  * **AndrOpen Office**: Outdated OpenDocument support, only partly functional.

Alas, many remaining glitches cannot be fixed without breaking SFCalcSheet in LibreOffice.

**Where can I see the equations?**

Most of the math is (invisibly) performed in the cells right of the calculator boxes. If you move the selection to those you can see the formula in the input line at the top of the window. However, the wiki has it conveniently [all on one page](https://github.com/lortordermur/sfcalcsheet/wiki/Formulas).

**I miss a specific calculator or feature.**

Great, and this can be helped! Just file an issue on [sfcalcsheet's issue tracker](https://github.com/lortordermur/sfcalcsheet/issues) and I will look into it.

**I cannot edit templates. The dialog simply does not open.**

To fix this you must unprotect all sheets. You can do so by selecting all tabs using shift-click and selecting `Tools->Protect Sheet` from the main menu.

**I would like to see the hidden interim calculations.**

This can be easily done by editing a format template. Bring up the template sidebar using the F11 key and right-click on the "InterimResult" template. Choose to edit, and on the text effects tab set the text color to anything other than black.
