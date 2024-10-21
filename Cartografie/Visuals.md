# Semiology 
	= Study of signs and symbols and their use or interpretation

|          Type           | Compatible Data Type |                                                   Extra Info                                                   |
| :---------------------: | :------------------: | :------------------------------------------------------------------------------------------------------------: |
|     **Shape/Form**      |     Qualitative      | Can be pictoral/associative/abstract<br>Associative: shape suggests feature symbolized (triangle for mountain) |
|        **Size**         |     Quantitative     |                                                                                                                |
|     **Orientation**     |       Nominal        |                                            Direction of the symbols                                            |
| **Perspective height**  |  Interval and ratio  |                                    Less used (for eg. population of states)                                    |
|       **Spacing**       |     Quantitative     |                                          Changes in distance between                                           |
|     **Arrangement**     |       Nominal        |                                                                                                                |
|    *Color*: **Hue**     |         All          |                               Appropriate for nominal data (eg. blue for water)                                |
| *Color*: **Lightness**  |     Quantitative     |                                      Light = smaller value, dark = larger                                      |
| *Color*: **Saturation** |     Quantitative     |                                       How pure the color is (grayscale)                                        |
## Quantitative Data
Suitable if its easy to see **big-small, high-low, dark-light patterns**
## Qualitative Data
Suitable if no clear hierarchy (eg. river or building)
## Perceptual Effects
Perception might be influenced by other aspects of the map
# Colors
## Purpose
- **Clarification** main message (eg. land vs water)
- **Highlight** information (deep vs shallow water)
- Show **variations** in data

Often culture-dependent but several *universal*:
- Warm colors: red/orange/yellow
- Cool colors: blue/purple/green
-> temperature uses *warm for hot areas* and *cool for colder*

***Check for cultural meaning if you are mapping for global audience***
## Models
- **Additive**: color by adding or transmitting light (eg. in digital screens)
- **Subtractive**: color by light absorption or reflection (eg. in printing)
## Dimensions
### Hue
Sensation we perceive when light of a **specific wavelength** reaches eye
### Brightness
How **dark or light** color is with a constant hue
### Saturation
Purity, intensity, **colorfulness** of a hue
## Color Models
### Hardware-oriented
#### RGB
- **Additive**
- Defined by portions of R,G and B (up to 256)
	- [p] Relates nicely to *method on display*
	- [c] Hue, saturation and lightness not inherent
	- [c] Equal steps do not correlate to equal visual steps 
#### CMY(K)
- **Subtractive**
- Like mixing ink
- Same pros/cons as RGB
- *K-variant*: black as additional color
### User-oriented
#### HSV/HSB
	= Hue, Saturation, Brightness/Value
- Projected on circle, higher saturation near edge
#### Munsell System
### CIM (neither hardware or software)

## Color Schemes
### Quantitative Schemes
#### Sequential Schemes
- **Lightness for ordered data**
	- Darker for higher data values
- Include hue differences to provide contrast between colors
- 3-9 classes to keep them distinct
#### Diverging Schemes
- Emphasize both **high and low** values
	- mean values in lighter color
	- extremes more dark hues
### Qualitative Schemes
For unordered features (**nominal data**); varying hues

>[!Error] Waarschuwing
>A well defined qualitative scheme should NOT suggest that data is ordered

If *logical relationships* exist -> *echo* them with related colors
**Use color conventions** if applicable (blue - water; green - forest)
# Texts
## Purpose
- **Label**
- Explain, direct or point
- **Establish hierarchy** or show size
## Typography (font)
### Type/Family
**Serif**:  used in books and articles
**Sans serif** (non-serif)
**Handwriting**: no longer used

![[{EC15D227-49B8-4832-91FF-3820A5355484}.png|Serif Type Fonts]]

**Letter width** dependent on family used
### Letter Spacing
	= Amount of space between characters
**Letter kerning**: adjusting space between individual letter forms
### Text Orientation
![[{567FC56A-614B-4840-A530-283C633EA1CB}.png|350]]
### Color of Text
**Lightness** might suggest **importance**
***Basic color guidelines still applicable***
### Special Effects
**Masks**: rectangles/box/border with background
**Callouts**: masks with *lines that point to features*
## Text Placement
###  Principles
- Must be **undoubtful**
- **Readable**; not too small, not too big, keep seperated from surrounding text
### Point Features
Order of **preference** from *1 to 6*:
- Better to *shift up/down* than to align them with point (between 1/2 or 3/4)
- Prefer to ***not overlap other features***
	- Unless using mask to keep readability

![[{8F786DCE-0704-4BCA-A46E-C02C1DA5E037}.png|475]]

**Masks**:  rectangles placed under the types, creating special space for lettering
**Halo**: extends outline of letters like a drop shadow

### Line Features
#### Principles
- Try to **follow curve**
- ***Along or inside*** object
- Repeat name when unclear
#### Example
````col
```col-md
flexGrow=1
===
### Before
![[{564B1E35-226F-4247-88B1-7FDD972F1F27}.png]]
```
```col-md
flexGrow=1
===
### After
![[{920C5F3E-ECD4-4C81-B06C-2E7810D20383}.png]]
```
````
### Area Features
#### Principles
- **Inside**
- Try to **follow shape** or use callout
- Can *stretch labels for bigger area*
- **Avoid conflicts** between features
#### Problems
**Automatic text placement** is complex issue
-> *manually improve* outcome
Avoid dense label placements and trade-offs between rules
# Design Principles
