# Map
## Definition

*Symbolised* **representation** of geographical **reality**
## Characteristics

- **Abstract** view to reality
- **Simplifies** complex **reality**
- Represents **various space types**
	- *Geographic* (area, statistical data)
	- *Planet*
	- *Non-geographic* (eg. subway map)
	- *Mental*
## Functions
- Recording and storing **information**
	- Topographical
	- Cadastral (land ownership)
	- World views
	- National identifier
- ***Analysing geographical data***
- **Presenting** information and communicating findings
- **Navigation** aid
## Categories
````col
```col-md
flexGrow=1
===
### By Purpose:
- Topographic maps or reference maps
- Thematic maps
- Navigation maps
```
```col-md
flexGrow=1
===
### By Organization:
- Individual map
- Map series
- Atlas
```
````

By **usage format**: paper/computer
By **usage context**: stationary/mobile
By **date**: old/historical, actual

**Map cube** used in *academic context*:
- *Audience*: public/private
- *Information* presented: known/unknown
- *Human-map interaction*: low/high
# Cartographic Process
## Model
**Kolacny's model**: most used

### Cartographic design
1. **Projection** (flatten 3D surface to 2D)
2. **Symbolization**
3. **Generalization**
# Geographic Data and Phenomena
## Phenomena Types
- **Geographic**: features that are mapped
	- *Point*: house, tv tower
	- *Line*: river
	- *Areal*: farm, lake
	- *Volume*
- **Physical**:
	- Tangible: buildings, rivers,...
	- Intangible: air masses, temperature...
	- Transient: earthquakes
- **Abstract**: concepts (population density)
- **Process-based**: changes (eg. land use evolution)
## Data Types
- **Qualitative**
	- *Nominal*: no order or ranking
	- *Ordinal*: ranked categories (eg. small, medium, large)
- **Quantitative**
	- *Interval*: no real zero point
	- *Ratio*: fixed origin or zero point
	- *Discrete*: 

> [!Info]
> ### Usage in portraying data
>![[{0E9BF39F-6A50-466C-85F9-AD6308539D14}.png]]
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

> [!Example]
> ````col
>```col-md
> flexGrow=1
> ===
> ### Before
> ![[{564B1E35-226F-4247-88B1-7FDD972F1F27}.png]]
> ```
> ```col-md
> flexGrow=1
> ===
> ### After
> ![[{920C5F3E-ECD4-4C81-B06C-2E7810D20383}.png]]
> ```
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
- ***Simplicity***: reduce unnecessary complexity
- ***Effectivity***
- ***Conventions***
## In Cartography
***Important things should look important***:
- **Visual hierarchy**
	-> order elements according to importance
- **Contrast**
	-> make sure differences can be easily seen
- **Figure-ground**
	-> visual prominence of *figure vs background*
- **Readability**
	-> make symbols big enough to allow comfortable reading
# Scale, Map Generalization
## Scale Types
- Fraction
- Bar scale
- Variable bar scale (diff in latitude vs longitude measurements)
## Map Generalization
	= Reducing information content because of scale, purpose, audience

**Preserve main characteristics**
-> all maps are generalized to some degree

### Model for Generalization
- **Why** (conceptual objectives)
	- **Reasons**: readability, scale, purpose, audience
- **When** (cartometric evaluation)
	- Reasons
		- Congested features
		- Coalescence (features overlapping due to scale)
		- Conflict (feature inconsistency)
		- Compilation
	- Considerations
		- Density, difference, purpose, quality...
- **How** (fundamental operations)
	- Selection/elimination (give priority)
	- Symbolization
	- Classification
	- Aggregation
	- **Graphic simplification** (eg. smoothing out lines)
		- Douglas-Peucker
	- **Graphic exaggeration** (important parts are enlarged)
	- **Graphic displacement** (move unimportant objects away to make space for improtant ones)
### Algorithms and Automatic Map Generalization
````col
```col-md
flexGrow=1
===
### Algorithms
#### Considerations
- Shape
- Area
- Relative distribution density
- Topological relationships
	- Within, touches, crosses, overlaps...
#### Types
- **Horton's orders**
	- Relative *importance stream segments* (eg. remove cat. 3 segments)
- **Douglas-Peucker**
	- Simplify line while keeping main points
```
```col-md
flexGrow=1
===
### Automatic Generalization Workflow
1. Divide map in small chunks
2. Begin with most important type
3. Begin with operations that have no graphic conflict
4. Reiterate

#### Difficulties
Other dependencies 
Retroactive effect of previous decisions

```
````
# Topographic Maps
	= Visual recording of landscapes based on measurements
## Representations
- **Terrain**
- **Landscape** configurations (settlements, transport networks, hydrography, landcover...)
- **Toponyms** (names of places, features)
## Functions
- Represent **spacial configurations**
- Relationships, topology, connectivity
- Distances, directions, areas
- Tool to identify problems
## Requirements
- Completeness
- Accuracy
- Equal visual importance of map feature types
- Clarity
# Representation of terrain and elevation
**Elevation**: height or depth of terrain compared to eg. mean sea level
**Relief**: changes in elevation in area
## Measurement
- Levelling, GPS, Radar, LIDAR
- **Benchmark points** on ground
- T.A.W. (Tweede Algemene Waterpassing) reference points
## Models
- **Contour lines**: lines connecting equal elevation points
	- **Isobaths**: *depth contours* under water
- **Hachure**: short lines in *direction of steepest hill gradient*
- **Shaded relief**: by shadowing based on light source (typically from NW)
- **Hypsometric tinting**: color of hues representing terrain
- **Oblique views**
	- *Panorama* map views
	- Draped images
- Physical models
# Map Projections
	= Systematic and orderly representation of the earths grid on a plane
 Developable Surfaces (*plane, cylinder, cone*)
## Distortions
### Types
- **Distance**
	-> equidistant
- **Area** 
	-> equivalent
- **Angle** 
	-> conformal
- Compromise (everything)
### Tissot's indicatrix
	= visualization to analyse distortions
Circle on sphere, ellipse on projected map
**Main axes of distortions**: *axes that are perpendicular before and after projection*
## Quantifying distortions
````col
```col-md
flexGrow=1
===
### Distance
![[Pasted image 20241205161731.png]]
```
```col-md
flexGrow=1
===
### Angle
![[Pasted image 20241205161835.png]]
```
```col-md
flexGrow=1
===
### Area
![[Pasted image 20241205161819.png]]
```
````

## Orthogonal Map Projections
**Medians perpendicular to parallels**
-> median and parallels are main axes of distortion
So: distance distortians along medians and parallels

### Distance Distortion
![[Pasted image 20241205162623.png]]
## Equidistant Map Projections
Equidistant only **in one direction**
-> meridians: h = 1
-> parallels: k = 1

## Applications
- **Equidistant Azimuthal**
- **Orthographic Azimuthal**
- **Equidistant cylindrical**
- **Equidistant conic**
## Equivalent Map Projections
- **Preserving area**, *not shape*
### Applications
- **Lambert azimuthal equivalent**: k > 1; h < 1
- **Gall-Peters** : cylindrical; k < 1; h > 1
## Conformal Map Projections
- **Preserving angles**: *preserving shapes*
### Applications
- **Stereographic azimuthal**
- **Mercator** (cylindrical)
- **Lambert conic conformal**
## Compromise Map Projections
- Hybrid between 3 above, for aesthetics or if compromise is desired
### Applications
- **Gnomonic Azimuthal**: h > 1; k > 1
	- Shows *shortest distance as straight line*
	- Used for navigation
## Transformation
		2 types: coordinate and datum transformation
### Coordinate Transformation
Convert between different coordinate systems (Geographic, Projected)

Steps:

1. Map coordinates to geographic coordinates (inverse projection)
2. Geographic coordinates to new map coordinates (projection)

OR

1. Map coordinates to geographic
2. **Molodensky** or **regression transformation** to geographic
3. Geographic to new map coordinates
### Datum Transformation
Align data between different reference surfaces

Steps:

1. Map coordinates to geographic
2. Geographic to **geocentric**
3. Geocentric to **new geocentric**
4. New geocentric to geographic
5. Geographic to new map coordinates
## Selecting a Map Projection
Based on **factors**
-> most critical factors have priority

eg. conformal projection for navigation (angles)
eg. equivalent projection for distribution (area)
# Thematic Mapping
