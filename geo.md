
**Mehdi Zamani** 16:15
In Python with geopy, we should consider two separate issues:

1. **Coordinate order**

geopy expects coordinates as:

```
(latitude, longitude)
```

However, some datasets use:

```
(longitude, latitude)
```

For longitude-first data, convert it using:

```
from geopy.distance import lonlat

point = lonlat(longitude, latitude)
```

1. **Distance-calculation method**

```
from geopy.distance import geodesic, great_circle
```

* geodesic: More accurate; uses an ellipsoidal Earth model and is the default.
* great_circle: Uses a spherical Earth model and may have an error of up to approximately 0.5%.

For accurate calculations, use:

```
distance = geodesic(
    (latitude_1, longitude_1),
    (latitude_2, longitude_2)
).km
```
