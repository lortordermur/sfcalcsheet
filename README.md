**SFCalcSheet** – Science Fiction Calculation Spreadsheet


### Summary ###

A LibreOffice spreadsheet for performing various science fiction related calculations.


### Included sheets and functions ###

* **Constants**: Collection of physical constants used in the spreadsheet's internals.
* **Star**: Star related calculators.
  * Magnitude <-> luminosity
  * Magnitude/distance
  * Luminosity difference
  * Star properties
* **Planet**: Planet calculators.
  * Physical properties
  * Orbital properties
  * Planetary habitability
  * Population density
  * City area
* **Satellite**: Calculators pertaining to natural satellites, i.e. moons.
  * Satellite appearance
  * Satellite orbit
* **Impact**: Impact calculators.
  * Impact and crater
* **Travel**: Space travel calculators.
  * Light years <-> parsec
  * FTL factor
  * FTL travel time
  * Time dilation
  * m/s <-> km/h
  * Uniform acceleration


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


### Frequently asked questions ###

**I cannot edit templates. The dialog simply does not open.**

To fix this you must unprotect all sheets by right-clicking on each one's tab and selecting the appropriate option in the pop-up menu.

**I would like to see the hidden interim calculations.**

You can do so by editing a format template. Bring up the template sidebar using the F11 key and right-click on the "InterimResult" template. Choose to edit, and on the text effects tab set the text color to anything other than black.
