![SFCalcSheet logo](logo.png)

**SFCalcSheet** – The science fiction calculation spreadsheet

**[Download](https://github.com/lortordermur/sfcalcsheet/releases/latest) · [Screenshots](https://github.com/lortordermur/sfcalcsheet/wiki/Screenshots) · [How-tos](https://github.com/lortordermur/sfcalcsheet/wiki/How%E2%80%90tos) · [Formulas](https://github.com/lortordermur/sfcalcsheet/blob/master/formulas.pdf)**


### Summary ###

This is a cross-suite spreadsheet for performing various science fiction and astronomy related calculations. The aim is to cover all common math problems in SF while keeping it simple for the user. The spreadsheet can assist with worldbuilding in science fiction and fantasy, or be used as an aid in amateur astronomy.

While being developed and maintained in [LibreOffice Calc](https://www.libreoffice.org), SFCalcSheet also works nicely in a number of additional office suites including [Google Sheets](https://docs.google.com/spreadsheets), [Excel Online](https://www.office.com/launch/excel) and [Collabora Office](https://www.collaboraoffice.com/).

To get started you can check out the [releases page](https://github.com/lortordermur/sfcalcsheet/releases), [some screenshots](https://github.com/lortordermur/sfcalcsheet/wiki/Screenshots), or [browse the formulas](https://github.com/lortordermur/sfcalcsheet/blob/master/formulas.pdf) that are used in the spreadsheet. There are a few [how-tos](https://github.com/lortordermur/sfcalcsheet/wiki/How%E2%80%90tos) too. If you would like to share informal feedback or constructive criticism, there are an [official Reddit thread](https://www.reddit.com/r/worldbuilding/comments/iodfba/sfcalcsheet_science_fiction_calculation) and a [Discord channel](https://discord.gg/TTumbhQ) as well.


### Included calculators and converters ###

* **Constants**: Collection of physical constants used in the spreadsheet’s internals.
* **Conversion**: Unit conversion.
  * Light years <-> parsec
  * km <-> AU
  * m/s <-> km/h
  * HMS <-> degrees
  * Degrees <-> radians
  * Equatorial <-> galactic coordinates
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
  * Stellar evolution
  * Stellar wind
  * Binary orbit
* **Planet**: Planet calculators.
  * Mass converter
  * Physical properties
  * Orbital properties
  * Tidal forces
  * Ring system
  * Planetary albedo
  * Planetary habitability
  * Population density
  * City area
* **Satellite**: Calculators pertaining to natural satellites, i.e. moons.
  * Satellite appearance
  * Satellite orbit
  * Lunar habitability
* **Compact**: Compact object calculators.
  * Schwarzschild black hole properties
* **Disaster**: Disaster calculators.
  * Impact and crater
  * Neutron matter explosion
  * Matter/antimatter annihilation
  * Bomb blast
  * Earthquake
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
  * 3D distance
  * Terrestrial travel time


### Write protection ###

To avoid overwriting the default values by an accidental save, the spreadsheet file can be write protected in Unix-like environments using `chmod 444 sfcalcsheet.ods`. These permissions allow for the file to be opened for editing (you might get an additional prompt for this) but it cannot be saved back to the same file. You can make the file writable again with `chmod 664 sfcalcsheet.ods`.


### Caveats ###

SFCalcSheet attempts to keep algebraic complexity on a manageable level for the sake of maintainability. The following formulas are simplistic approximations and should not be used for work requiring scientific accuracy:

* Star radius
* Star temperature
* Star habitable zone
* Stellar wind and mass loss
* Roche limit
* Albedo of planetary rings
* Greenhouse effect part of planetary temperature
* Interaction of planetary/lunar magnetic fields
* Black hole lifetime
* Impact crater size
* Bomb blast fireball radius
* Vegetation color
* Vehicle mass


### Frequently asked questions ###

#### How do I get the spreadsheet downloaded and running? ####

To obtain the zipfile containing the SFCalcSheet distribution, click on the [latest release](https://github.com/lortordermur/sfcalcsheet/releases/latest) in the right-hand sidebar. On the release page click the “sfcalcsheet-vx.xx.zip” file under “assets”. Download this file to a subfolder in your usual download location and unpack it. If you have an office suite installed (such as Microsoft Office or [LibreOffice](https://libreoffice.org)), open sfcalcsheet.ods and you are done. Should this not work, but you have Google Drive or OneDrive, save sfcalcsheet.ods to it, then click the uploaded file to open it in the respective web-based office suite.

Here is [a comprehensive how-to](https://github.com/lortordermur/sfcalcsheet/wiki/How%E2%80%90to%3A-Download-and-run-SFCalcSheet).

#### How can I stay updated about new releases? ####

The easiest way to not miss out on SFCalcSheet releases is to subscribe to the [Atom feed](https://github.com/lortordermur/sfcalcsheet/releases.atom) or follow me [on Twitter](https://twitter.com/lortordermur). Alternatively you can join the [Discord channel](https://discord.gg/TTumbhQ) which will notify you of any commits to the repository.

#### Not all calculators from the list are in the spreadsheet, why? ####

The README file follows the development version of SFCalcSheet so features may be mentioned that were not yet in the latest release. To get the development version click the green “code” button at the top of the web page and then "download ZIP", or alternatively download sfcalcsheet.ods directly from the file list.

#### Does it really work in office suites other than LibreOffice? ####

Yes, but in several cases only with serious flaws that cannot be fixed in the spreadsheet. SFCalcSheet uses some pretty fancy OpenDocument functions and cell styles, and therefore cannot be guaranteed to fully function in every office software. Apart from LibreOffice it has been tested in the following office suites featuring OpenDocument support:

* **Desktop software**

  * **Collabora Office**: Based on current LibreOffice. ***Completely functional*** without visual glitches.
  * **SoftMaker Office**: Well-functioning but calculator headings don’t show, as well as some background colors in random places.
  * **SoftMaker FreeOffice**: Outdated OpenDocument support, only partly functional.
  * **Microsoft Excel**: ***Near-completely functional***. The only broken parts are the display of star color temperature and the height of word-wrapped cells.

* **Web applications**

  * **Google Sheets**: ***Completely functional*** after post-v0.09 fixes. Visual glitches with framed cells.
  * **Microsoft 365**/**Excel Online**: ***Near-completely functional*** after post-v0.10 fixes. Same glitches as in the desktop suite.
  * **Zoho sheet**: Mostly functional but calculator headings don’t show, and calculators using the IFS function (such as “Simple calculator” and “Structure properties and resources”) don’t work properly.

* **Android apps**

  * **Collabora Office**: Same engine as the desktop software, ***completely functional***.
  * **Google Sheets**: Same engine as the web application, ***completely functional***.
  * **Excel/Microsoft Office**: Outdated OpenDocument support, only partly functional.
  * **AndrOpen Office**: Outdated OpenDocument support, only partly functional.
  * **Zoho Sheet**: Same engine and glitches as the web application.
  * **PlanMaker**: Calculator headings don’t show, special characters are not represented, glitched up footnote color, otherwise functional.
  * **OpenDocument Reader**: All text displayed white on black, editing non-functional.
  * **ONLYOFFICE documents**: Input text and most result text displayed in black, only partly functional.

* **iOS apps**
  * **Microsoft Excel**: Same engine and glitches as the web application, ***near-completely functional***.

Alas, many of the remaining glitches cannot be fixed without breaking SFCalcSheet in LibreOffice, because OpenDocument support is oftentimes outdated or incomplete.

#### SFCalcSheet looks broken in Google Sheets. ####

OpenDocument support in Google Docs has been worsening recently. A workaround is to export SFCalcSheet to .xlsx format in LibreOffice or Collabora Office and upload that exported file instead.

#### Where can I see the equations? ####

Most of the math is (invisibly) performed in the cells right of the calculator boxes. If you move the selection to those you can see the formula in the input line at the top of the window. However, the formulas PDF file has it conveniently [all in one place](https://github.com/lortordermur/sfcalcsheet/blob/master/formulas.pdf).

#### What are those 12.34E+56 numbers about? ####

It is scientific exponential notation for very large and very small numbers. “E” is a shorthand for “ten to the power of”. Hence, 12.34E+56 is identical to 12.34 ✕ 10⁵⁶, and 12.34E-56 is identical to 12.34 ✕ 10⁻⁵⁶.

#### I am tired of typing sizable numbers with lots of zeros. ####

Fortunately, the aforementioned exponential notation is available in every numerical input field in SFCalcSheet. If you need to do some preparatory math before keying in the values, use the “Simple Calculator” on the Conversion sheet or type your calculation into [Google](https://www.google.com) or [Wolfram Alpha](https://www.wolframalpha.com).

#### I miss a specific calculator or feature. ####

Great, and this can be helped! Just file an issue on [SFCalcSheet’s issue tracker](https://github.com/lortordermur/sfcalcsheet/issues) and I will look into it.

#### I cannot edit cell styles. The dialog simply does not open. ####

To fix this you must unprotect all sheets. You can do so by selecting all tabs using shift-click and selecting `Tools->Protect Sheet` from the main menu.

#### I would like to see the hidden interim calculations. ####

This can be easily done by editing a cell style. Bring up the styles sidebar using the F11 key and right-click on the “InterimResult” style. Choose to edit, and on the font effects tab set the text color to anything other than black.

#### Some cells containing large results are too narrow for their content. What can I do? ####

Unlock the current sheet using `Tools->Protect Sheet` and then use the handles on the column bar to adjust the width.

#### Long footnotes appear cut off in the calculators. ####

This is a known issue in Excel and there is currently no fix for it. To see the whole text, select the cell with the footnote so you can read the text from the input line at the top of the window.

#### What is that nice sans font in the LibreOffice screenshots? ####

It is SFCalcSheet’s default font, [DejaVu Sans](https://dejavu-fonts.github.io). It comes preinstalled on most desktop Linux distributions.

#### How can I send you a private message? ####

For this, please message [/u/lortordermur](https://www.reddit.com/user/lortordermur) on Reddit or [lortordermur](https://twitter.com/lortordermur) on Twitter. You can also message me on my [Discord server](https://discord.gg/TTumbhQ).


### How you can support the project ###

There are a couple of ways you can participate and help:

* Leave some feedback, praise or anecdotes [on Reddit](https://www.reddit.com/r/worldbuilding/comments/iodfba/sfcalcsheet_science_fiction_calculation) or [Discord](https://discord.gg/TTumbhQ).
* Request a specific calculator or feature.
* Post some useful formulas in the Reddit thread or in the Discord channel and maybe I will turn them into a calculator.
* [Star](https://github.com/lortordermur/sfcalcsheet/stargazers) SFCalcSheet on GitHub.
* [File an issue](https://github.com/lortordermur/sfcalcsheet/issues) on GitHub for a long-standing quirk or wanted feature.
* Test and/or debug SFCalcSheet on various office suites, and post the results in the Reddit thread or on Discord.

### Licenses used ###

Project files: [The Unlicense](https://unlicense.org/)

Logo background: [Creative Commons CC0](https://creativecommons.org/publicdomain/zero/1.0/deed.en); image source: [An artist's rendering of a planet in the sky. Lunar landscape star brown dwarf, science technology.](https://picryl.com/media/lunar-landscape-star-brown-dwarf-science-technology-c91acf)
