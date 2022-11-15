## Homework: feast

A chef is planning a magnificent feast consisting of a sequence of dishes. Each dish can only be served once. Each dish tastes spicy, sour, salty, sweet, umami or bland. Each dish is served hot, cold or warm. Each dish is either heavy on the stomach or light.

* The chef would never serve two dishes of the same taste in a row, that would be boring. 
* The first dish should be salty, and the last dish should be sweet. 
* After a spicy dish the next dish must be bland or sweet. 
* After a sour dish the next dish must be bland or umami. 
* No spicy or umami dishes can go directly after a sweet dish.
* Between serving a hot dish and a later cold dish there must be a warm dish.
* The feast cannot have more than 2 heavy dishes in a row.

The magnificence of the feast, which we want to maximize, is given by the sum of the value of the dishes, plus the number of changes in taste, temperature and "weight" between each pair of consecutive dishes.

Try to use the constraint `regular` at least once. Running
```
picat feast.pi instance.pi
```
for the provided sample instance `instance.pi` should output the magnificence value of `41` and the sequence of dishes, one possibility is `[charsiubao, laiwongbao, glassnoodles, sesameprawn, mapotofu, coconutjelly]`.