**SFCalcSheet** – Science fiction calculation spreadsheet for LibreOffice


### Summary ###

This is a LibreOffice Calc spreadsheet for performing various science fiction and astronomy related calculations. The aim is to cover all common math problems in SF while keeping it simple for the user. The spreadsheet can assist with world-building in science fiction and fantasy, or be used as an aid in amateur astronomy.


### Included calculators and converters ###

* **Constants**: Collection of physical constants used in the spreadsheet's internals.
* **Star**: Star related calculators.
  * Magnitude <-> luminosity
  * Magnitude/distance
  * Luminosity difference
  * Star color
  * Star properties
* **Planet**: Planet calculators.
  * Mass converter
  * Physical properties
  * km <-> AU
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
* **Creature**: Calculators related to living beings.
  * Body weight
* **Structure**: Calculators for large structures.
  * Structure properties and resources
* **Vehicle**: Vehicle calculators.
  * Vehicle mass and personnel
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
* Vehicle mass


### Frequently asked questions ###

**I miss a specific calculator or feature.**

Great, and this can be helped! Just create an issue on [sfcalcsheet's issue tracker](https://github.com/lortordermur/sfcalcsheet/issues) and I will look into it.

**I cannot edit templates. The dialog simply does not open.**

To fix this you must unprotect all sheets. You can do so by selecting all tabs using shift-click and selecting `Tools->Protect Sheet` from the main menu.

**I would like to see the hidden interim calculations.**

This can be easily done by editing a format template. Bring up the template sidebar using the F11 key and right-click on the "InterimResult" template. Choose to edit, and on the text effects tab set the text color to anything other than black.
