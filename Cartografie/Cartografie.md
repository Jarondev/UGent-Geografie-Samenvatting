# Cartographic Process
## Model
**Kolacny's model**: most used
### Cartographic design
1. **Projection** (flatten 3D surface to 2D)
2. **Symbolization**
3. **Generalization**
# Geographic Data and Phenomena
## Data Types
- **Qualitative**
	- *Nominal*: no order or ranking
- **Quantitative**
	- *Ordinal*: ranked categories (eg. small, medium, large)
	- *Interval*: no real zero point
	- *Ratio*: fixed origin or zero point

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
**Quantitative Data**: suitable if its easy to see **big-small, high-low, dark-light patterns**
**Qualitative Data**: suitable if no clear hierarchy (eg. river or building) 
**Perceptual Effects**: perception might be influenced by other aspects of the map
# Colors
## Models
- **Additive**: color by adding or transmitting light (eg. in digital screens)
- **Subtractive**: color by light absorption or reflection (eg. in printing)
## Color Models
### RGB
- **Additive**
- Defined by portions of R,G and B (up to 256)
	- [p] Relates nicely to *method on display*
	- [c] Hue, saturation and lightness not inherent
	- [c] Equal steps do not correlate to equal visual steps 
### CMY(K)
- **Subtractive**
- Like mixing ink
- Same pros/cons as RGB
- *K-variant*: black as additional color
## Dimensions
**Hue**: sensation we perceive when light of a **specific wavelength** reaches eye
-> *quantitative*
**Brightness**: how **dark or light** color is with a constant hue
-> *qualitative*
**Saturation**: purity, intensity, **colorfulness** of a hue
-> *qualitative*
# Texts
## Typography (font)
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
**Automatic text placement**
-> *manually improve*

# Design Principles
***Important things should look important***:
- **Visual hierarchy**: order based on importance
- **Contrast**: differences stand out
- **Figure-ground**: visual prominence of *figure vs background*
- **Readability**: adjust size for reading
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
- **How** (***fundamental operations***)
	- Selection/elimination (give priority)
	- Symbolization
	- Classification
	- Aggregation
	- **Graphic simplification** (eg. smoothing out lines)
		- Douglas-Peucker
	- **Graphic exaggeration** (important parts are enlarged)
	- **Graphic displacement** (move unimportant objects away to make space for improtant ones)
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
# Map Projections
	= Systematic and orderly representation of the earths grid on a plane
 Developable Surfaces (*plane (azimuthal), cylinder, cone*)
## Distortions
### Types
- **Distance**: equidistant
- **Area**: equivalent
- **Angle**: conformal
- Compromise (everything)
## Azimuthal Map Projections
To **preserve direction** from center point, other properties are distorted
-> for navigation

**Medians perpendicular to parallels**
-> median and parallels are *main axes of distortion*
So: distance distortians along medians and parallels
## Equidistant Map Projections
To **preserve distance** from center point, distort area and shape with distance
-> for mapping routes from central location

Equidistant only **in one direction**
## Equivalent Map Projections
To **preserve area**, *not shape*
-> for thematic maps and comparing data distributions
### Applications
- **Lambert azimuthal equivalent**: k > 1; h < 1
- **Gall-Peters** : cylindrical; k < 1; h > 1
## Conformal Map Projections
To **preserve angles**: *preserving shapes*, distort area further from central point
-> for navigation, meteorology and other
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
## Selecting a Map Projection
Based on **factors**
-> most *critical factors have priority*

eg. conformal projection for navigation (angles)
eg. equivalent projection for distribution (area)
# Thematic Mapping
## Summary
![[Safari _ 19-12-2024_0141PM@2x.png]]
![[Safari _ 19-12-2024_0140PM@2x.png]]
![[Safari _ 18-12-2024_1059PM@2x.png]]

## Data classification Techniques
- *Classed*: grouped into classes with value range
	- *Equal interval*
	- *Quantiles*: each class has same number of area units
	- *Mean-standard deviation*: groups data based on how far values deviate from median
	- *Optimal* (median): divides data to minimize difference within each class based on median
		- Natural breaks based on algorithms
	- **Number of classes**
		- Depending on map theme, data pattern and complexity
		- *Typically 7 +/- 2* (*algorithms exist* to find optimal amount)
		-> **outliers often seperated** from dataset
- *Unclassed*: color assigned proportionally to each data value
	-> more accurate results but harder to interpret
## Choropleth Maps
````col
```col-md
flexGrow=1
===
Distinctive color or shading applied to **statistical or administrative areas**
- To represent magnituted/values of attributes in area
- Often well-defined and known areas
```
```col-md
flexGrow=1
===
![[Pasted image 20250118160528.png]]
```
````


Appropriate for phenomenon uniformly distributed within area and **changes at boundary**
-> eg. GDP

Use ***equivalent map projection***

**Bivariate and multivariate maps**: mapping more geographical phenomena together
-> eg. combining into color matrix
### Issues to consider
**Normalize data** to make comparable (eg. percentage of area instead of raw number)

**Areal Symbolization**
- *Visual variable*: color lightness
- *Visual hierarchy*: important things should look important
- *Legend issues*: symbols first, then definition, ranked low to high

Adding **other references: to enhance interpretation** (eg. city names)
## Dasymetric Maps
**Refinement** of statistical data **using secondary data**
-> follow technique in choropleth maps
- Can show *variations within statistical area units*
Secondary data sources: land cover, use, elevation, coastlines, imagery....

***Quality depends on employed assumptions/rules and secondary data***

Steps:
1. Start with **choropleth map**
2. Get **ancillary data** for boundary refinement
3. **Re-compute and re-map**

> [!Example]
> ![[Safari _ 18-12-2024_0954PM@2x.png]]

## Dot Maps
````col
```col-md
flexGrow=1
===
Dots used to **communicate variation in spatial density**
-> Use **equivalent map projection**

Types:
- **One to one** (*nominal point thematic map*): 1 dot for 1 occurrence
	- Often qualitative data
- **Many to one** (more often used): 1 dot for multiple occurrences
```
```col-md
flexGrow=1
===
![[Safari _ 18-01-2025_0416PM@2x.png]]
```
````


**Advantages**: easy to understand, effective, show density depending on additional data
**Disadvantages**: perception of density not linear

### Data Suitability
- Normalized or ratio data should be ***avoided***
- Datasets with **large attribute ranges** are **more difficult** to visualize

### Considerations
**Size of area unit**
	- Use data at finest level
	- Show boundaries of areas at higher levels
**Dot value and size**: find balance
	- Coalescence in densest part
**Dot placement**: try to place *as close to real distribution* as possible
**Legend design**: multiple options
	 ![[Safari _ 18-12-2024_1012PM@2x.png|425]]

### Bivariate and multivariate dot maps
- Dots with **different color hues** to show **different phenomena**
- **Possible to combine** with other thematic map types
## Proportional Symbol Maps
Select **symbol form**, **vary size** in proportion to quantities it represents

For **quantitative data**

### Data Suitability
**True point data**: data measured at point locations (eg. passengers departing train station)
**Conceptual point data**: aggregated over area but shown as point at centroid (eg. population)
Less appropriate for:
- Interval data (eg. temperature)
- Densities
- Data with small and unchanging attributes
### Symbols
- Geometric (2D, 3D) -> <u>circles</u> commonly used
- Pictorial

Handle overlaps by putting **smaller on top of larger** or use **inset map**
### Scaling
**Scaling** *based on area* or volumes of symbol
-> difficult for pictorial
#### Continuous proportional scaling
Scale area based off comparing attribute to other points attribute

Area size is in proportion to radius of circle -> area * 4 = radius * 2
#### Range graded scaling
Based on **classes**, size scaled to **middle value** of each class
### Legend design
![[Safari _ 18-12-2024_1056PM@2x.png|625]]
### Bivariate and Multivariate proportional symbols
By eg. using pie charts instead of circles
![[Safari _ 18-12-2024_1058PM@2x.png|525]]
## Isarithmic Maps
````col
```col-md
flexGrow=1
===
Map showing **lines connecting points of equal value**
- Can **shade** or color area between
- For mapping **continuous and smooth phenomena**
	-> also heat maps

**Legend**: include text statement to indicate units, interval
```
```col-md
flexGrow=1
===
![[Safari _ 18-01-2025_0429PM 2@2x.png]]
```
````
### Selection of isarithmic intervals
<u>Dont</u> visualize isolines of all data values
Apply at **uniform interval** 

Steps:
1. Consider range of data
2. Experiment
3. Choose lowest isoline value

**Quality** depends on
1. point **data quality**
2. **number** of sample points 
3. **interpolation method** used

Data types: 
- **True point data** (*isometric*)
- **Conceptual point data** (*isoplethic*)
![[Safari _ 19-12-2024_0937AM@2x.png|525]]
### Requirements
1. Data is **continuous in nature** (*found everywhere in mapped area*)
2. Can be conceptualized in a geographic volume
3. Map designers must understand **distribution** being mapped
### Process
1. Collect or obtain point data at sample locations
2. **Interpolation**: estimate based on sample points
3. **Connect** locations of equal values using smooth lines (*isolines/contours*)
### Interpolation
**Linear interpolation**: assume *uniform linear distribution*
**Automated interpolation/gridding/surface modelling**: using interpolation methods
#### Interpolation methods
![[Safari _ 19-12-2024_1027AM@2x.png|500]]
1. **Linear triangulation**
	1. Create optimal set of triangles within sample data points
		- **Thiessen polygons** around sample points: points within polygon are closer to sample than nearby ones
	2. Contour lines by interpolating along edges
2. **Inverse Distance Weighted (IDW)**: weight based on distance to nearby points
	- *Neighborhood selection: which samples to use?*
		-> all/simple/quadrant/octant
		![[Safari _ 19-12-2024_1020AM@2x.png|375]]
		All: global; simple: within circle, quadrant..
## Dynamic Flow Map
````col
```col-md
flexGrow=1
===
Show linear **movement between places**
-> *actual items* (migration, export, trajectories) or *intangible things* (ideas, internet traffic)

**Qualitative flow**: show types of movement (what and where)
**Quantitative flow**: show quantity (what, where, how much)

Line **width or lightness** -> indicates **value** in quantitative flow maps

Legend: Mention **what and unit** if applicable, sometimes no legend needed

**Spiral tree**: show migration branches from central point
```
```col-md
flexGrow=1
===
![[Safari _ 18-01-2025_0430PM@2x.png]]
```
````


### Design
- Figure/ground contrast -> **(smaller) flow on top**
- Include *arrows* if direction is relevant
- Include comprehensive legend
#### Line Scaling
Unclassed: scale in **proportion** to represented quantities
Classed: if range is too big, scale based on applicable class
## Cartogram
**Size of area is proportional to data** value
For **ratio data**
### Contiguous Cartogram
Area units stay connected
-> shape more easily preserved

**Preserve shape** by generalizing/simplifying shape and keeping important features

For **small scale maps** (eg. world scale)
### Noncontiguous Cartogram
**Seperated area units**
-> more or less same location, with gaps

Easy to scale and construct, **preserves true shape**
Does not convey real geographic space, no overall compact form

**Variant: using circles (*Dorling*)**

### Construction
**Manual**
With **automated methods**
- Cartodraw, diffusion-based method, medial-axis based cartograms, fast flow-based method
# Multivariate Maps
Maps that **visualize two or more data variables** at the same time
**Legend design essential** for understanding meaning
### Encoding
**Inter-symbol encoding**: show both variables with distinct symbol
-> "combining" thematic map
**Intra-symbol encoding**: put both variables into one symbol (eg. size for one and color for other)
# Uncertainty Visualization
Types of uncertainty:
- **What**: attribute/thematic
- **Where**: location
- **When**: temporal


````col
```col-md
flexGrow=1
===
Can be **combined** with other data in multivariate map (eg. by hashed polygons)
Or use **more maps** to **compare** and illustrate range of possibilities
-> viewers can analyze and make their own conclusions
```
```col-md
flexGrow=1
===
![[Safari _ 18-01-2025_0432PM@2x.png]]
```
````

Reasons:
1. **ethical necessity**
2. can play **important role** in decision making