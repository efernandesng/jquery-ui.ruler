jQueryUI.Ruler
============

jQueryUI.Ruler is a jQuery-UI plugin that adds a photoshop-like rules to a DOM element.

## Features
- Multiple units (px, mm, cm, in)
- Three types of ticks (major, minor, micro)
- Mouse track
- Supports sub-divs

## Tasks
- [ ] Add support to more units
- [ ] Improve source-code

## Usage
```javascript
// simple initialization
$('.selector').ruler();

// or use different unit and tick values
$('.selector').ruler({
	unit: 'mm',
	tickMajor: 10,
	tickMinor: 5,
	tickMicro: 1,
	showLabel: true
});
```
## Documentation

###Options
**`unit`** Metric unit used by ruler.
_Default:_ **px**

unit    | Description
--------|------------
*px* | pixel
*mm* | millimeter
*cm* | centimeter
*in* | inch

**Example**
```javascript
// getter
var unit = $('.selector').ruler('option', 'unit');
// setter
$('.selector').ruler('option', 'unit', 'mm');
```
----------
**`tickMajor`** Interval of major tick. 
_Default:_ **100**
_Note:_ **0** to disable

**Example**
```javascript
// getter
var tickMajor = $('.selector').ruler('option', 'tickMajor');
// setter
$('.selector').ruler('option', 'tickMajor', '50');
```
----------
**`tickMinor`** Interval of minor tick. 
_Default:_ **20**
_Note:_ **0** to disable

**Example**
```javascript
// getter
var tickMinor = $('.selector').ruler('option', 'tickMinor');
// setter
$('.selector').ruler('option', 'tickMinor', '50');
```
----------
**`tickMicro`** Interval of micro tick. 
_Default:_ **10**
_Note:_ **0** to disable

**Example**
```javascript
// getter
var tickMicro = $('.selector').ruler('option', 'tickMicro');
// setter
$('.selector').ruler('option', 'tickMicro', '50');
```
----------
**`showLabel`** Show or hide major tick value 
_Default:_ **true**
_Note:_ **false** or otherwise to disable

###Methods
**`refresh()`** Refreshes all ruler components

**Example**
```javascript
$('.selector').ruler('refresh');
```
----------
##Licensing
**MIT**

##Similar projects
[jQuery.ruler](https://github.com/hilliuse/ruler/) - Add Photoshop-like rulers and mouse position to a container element using jQuery. [http://ruler.hilliuse.com](http://ruler.hilliuse.com)

[RulersGuides.js](https://github.com/mark-rolich/RulersGuides.js) - Creates Photoshop-like guides and rulers interface on a web page