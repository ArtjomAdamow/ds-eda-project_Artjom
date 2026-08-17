
# 1. Footage value vs. Neighborhood quality

>[!Hypothesis:]
> High footage property has an extreme increase of price towards the very center of a neighborhood; lowering the footage expectation might be a good trade off.

## Key Drivers of Central Price Surges
Property prices spike dramatically toward the center of a neighborhood due to high demand for scarce land, short commutes, and dense local amenities. This central core concentrates jobs, transit, and culture, creating an intense bidding war among buyers that drives up the cost per square meter far faster than in outer districts
* **Scarcity of Land:** Space right at the core is fixed, meaning new supply cannot match the surge in buyer interest.
* **Transit and Access:** Central spots minimize travel times and link directly to major job hubs.
* **Amenity Clustering:** Cafes, shops, and cultural sites sit within easy walking distance, raising perceived lifestyle value.
* **Economic Gravity:** High-income buyers and investors concentrate their capital here, setting a high baseline for what properties can command.

## count(house_id), price, sqft_lots, lat, long
find geographical concentration vs. footage and price

## sqft_lot15, sqft_living15
compare with neighborhood density for optimization


# 2. Building characteristics

>[!Hypothesis:]
> Older buildings have a unique charm, high ceilings and character; the financial and logistical burden towards energy-efficiency and comfort might be overrated, while the Landscape quality might be overrated.

## Financial Realities of Old Buildings
While un-renovated old buildings often have a lower initial purchase price, they frequently require high hidden modernization costs for energy efficiency, piping, and wiring. Upfront affordability can be offset by mandatory legal retrofits and expensive structural repairs.

* **Lower Purchase Price:** Un-renovated properties can cost significantly less upfront compared to new or fully modernized builds.
* **Renovation Expenses:** Bringing older systems up to modern code typically ranges from €800 to €1,800 per square meter depending on the condition.
* **Energy Mandates:** Outdated insulation and old heating systems often trigger legal remediation obligations under energy laws, driving up immediate post-purchase costs.
* **Hidden Structural Work:** Structural issues like damp cellars, old roofs, and outdated electrical wiring require deep investment beyond cosmetic fixes.

## find how does renovation influence the value?
yr_built, yr_renovated

## potential underrated criteria
grade, condition

## potential overrated price driving criteria 
view, waterfront


# 3. Building details

>[!Hypothesis:]
>Decimals mean added value to smaller footage property; features might be attractive for buyers with with medium and lower budget.

## Building floor Measurements

### Key Features of 1.5-Floor Layouts
A 1.5-story house features a full ground floor and a partial upper level under a sloped roof.
* **Main Level:** Contains the kitchen, living room, dining areas, and often the primary master suite.
* **Upper Level:** Offers smaller bedrooms, bathrooms, or open loft areas with sloped walls.
* **Exterior:** Characterized by roof dormers, gables, and lower eaves that reduce the home's vertical bulk.

### Calculation of floor area
Space Efficiency maximizes usable square footage and adds volume ceilings without the full cost or footprint of a two-story house.
* **Ceiling Height Rules:** Usable habitable rooms generally require a minimum ceiling height of 7 feet over at least half of the floor area.
* **Sloped Wall Calculation:** Floor space under sloped ceilings usually only counts toward official room size if the ceiling height reaches at least 5 feet.

## Bathroom Breakdown by Fixtures

* **Full bath (1.0):** Sink, toilet, tub, and shower.
* **Three-quarter bath (0.75):** Sink, toilet, and a shower (no tub).
* **Half bath / Powder room (0.5):** Sink and toilet.
* **Quarter bath (0.25):** Just a single fixture, typically a standalone toilet.
  A 1.25 rating is rare because a toilet room without a hand-washing sink violates some modern building codes or practical needs, but it may appear in older or multi-level historic homes


