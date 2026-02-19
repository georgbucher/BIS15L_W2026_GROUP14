# Butterfly host plant use driven by microclimate not nutritional quality

Dataset DOI: [10.5061/dryad.hqbzkh1wk](https://doi.org/10.5061/dryad.hqbzkh1wk)

## Description of the data and file structure

Data collected to support investigations into the role of microclimate around host plants and nutritional quality of host plants in shaping oviposition by a specialist herbivorous butterfly.  Each row in the dataset is a host plant, either a plant with one or more eggs or larvae (plant_id contains 'e') or a control plant next to an occupied plant (in a randomly selected direction) (plant_id contains 'c'). 

There are two datasets, one smaller dataset (plant chemistry data) which contains chemical data for a sample of host plants along with data on possible proxies for this chemical data. This data was used to identify the best proxies for host nutritional quality (nitrogen content).

The second larger dataset was then used for all further analyses. It contains data about host plant chemistry proxies, predicted host plant chemistry, the environment around them, the presence of butterfly eggs and larvae. 

The plants in the first dataset are largely a subset of those represented in the second, but several plants in the smaller dataset were later removed from the main analysis, and retained for the proxy analysis, hence the separate datasets.

### Files and variables

#### File: egg_laying_data.csv

**Description:** 

##### Variables

* predicted_n: Predicted nitrogen content of host plant, micromoles per g.
* n_se: standard error around predicted nitrogen content of host plant.
* n_weights: inverse of standard error around predicted nitrogen content of host plant.
* plant_id: unique identifier for host plant, a 'c' denotes a control plant, and 'e' a plant with butterfly eggs or larvae.
* id_number: numeric component of plant_id
* species: host plant species, all ra as all host plants were Rumex acetosa.
* season: season in which host plant was sampled, either autumn or spring (referred to as early summer in manuscript).
* n_eggs: number of eggs on plant
* larvae: number of larvae on plant
* occupied: whether the plant was occupied with butterfly eggs or larvae (based on preceding two columns).
* gps: British national grid reference of host plant
* bare_ground: %cover of bare ground around host plant, in 50cm grid with host plant at centre.
* veg: %cover of vegetation around host plant, in 50cm grid with host plant at centre.
* litter: %cover of litter around host plant, in 50cm grid with host plant at centre.
* sward_height: sward height (cm) around host plant, measured using direct method (see manuscript).
* plant_area: estimated area of host plant (in cm^2^, based on perpendicular dimensions of tightest fitting square - plant_size_1 multiplied by plant_size_2)
* bare: whether or not bare ground was present in the 50cm grid around the host plant.
* plant_size_1: One dimension of plant used to calculate plant area (cm).
* plant_size_2:  One dimension of plant used to calculate plant area (cm).
* leaf1_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf2_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf3_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf1_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf2_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf3_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf1_area: Area of a sampled leaf (mm^2^).
* leaf2_area: Area of a sampled leaf (mm^2^).
* leaf3_area: Area of a sampled leaf (mm^2^).
* total_leaf_area: Sum of areas of sampled leaves (mm^2^).
* leaves_sampled: Number of leaves from host plant sampled
* average_leaf_size: Average area of sampled host plant leaves (mm^2^)
* temperature_soil: Temperature measured at soil surface under host plant (degrees Celsius).
* temperature_ambient: Ambient temperature measured while measuring soil surface temperature under host plant (degrees Celsius).
* environment_date: Date on which environmental measurements for host plant were taken.
* temperature_date: Date on which temperature measurements for host plant were taken.
* date_mean_soil: Mean soil surface temperature of host plants measured on the same date as plant in that row.
* date_sd_soil: Standard deviation of soil surface temperatures of host plants measured on the same date as plant in that row.
* temperature_soil_scaled: Soil surface temperature under host plant, scaled and centred by sampling date to express whether a host plant was warmer or cooler than others measured on the same date.
* scaled_leaf_size: Centred and scaled average leaf area for host plant.
* scaled_n_content: Centred and scaled predicted nitrogen content for a host plant.

#### File: plant_chemistry_data.csv

**Description:** 

##### Variables

* plant_id: Unique identifer of host plant.
* N: % nitrogen content of host plant by mass
* C: % carbon content of host plant by mass
* cn_percent: Carbon : Nitrogen ratio of host plant by mass
* n_molar: Molar nitrogen content of host plant (micromoles per g).
* c_molar: Molar carbon content of host plant (micromoles per g).
* cn_molar: Molar Carbon : Nitrogen ratio of host plant
* plant_size_1: One dimension of plant used to calculate plant area (cm).
* plant_size_2:  One dimension of plant used to calculate plant area (cm).
* plant_area: Estimated area of host plant (in cm^2^, based on perpendicular dimensions of tightest fitting square - plant_size_1 multiplied by plant_size_2)
* leaf1_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf1_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf2_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf2_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf3_length: Length of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf3_width: Width of a sampled leaf used to calculate leaf area and average ultimately leaf size (mm).
* leaf1_area: Area of a sampled leaf (mm^2^).
* leaf2_area: Area of a sampled leaf (mm^2^).
* leaf3_area: Area of a sampled leaf (mm^2^).
* total_leaf_area: Sum of areas of sampled leaves (mm^2^).
* leaves_sampled: Number of leaves from host plant sampled
* average_leaf_size: Average area of sampled host plant leaves (mm^2^)
* season: Season in which host plant was sampled, autumn or spring (early summer in manuscript).
* quality_PC1: Value of first principal component of PCA of average leaf size and plant area for host plant.
* quality_PC2: Value of second principal component of PCA of average leaf size and plant area for host plant.

## Code/software

Datasets viewed in Microsoft excel, and analysed using R and R studio.
