## Homework: feast

A chef is planning a magnificent feast consisting of a sequence of dishes. Each dish can only be served once. Each dish tastes spicy, sour, salty, sweet, umami or bland. 

* The chef would never serve two dishes of the same taste in a row, that would be boring. 
* The first dish should be salty, and the last dish should be sweet. 
* After a spicy dish the next dish must be bland or sweet. 
* After a sour dish the next dish must be bland or umami. 
* No spicy or umami dishes can go directly after a sweet dish.

The magnificence of the feast, which we want to maximize, is given by the sum of the value of the dishes.

Use the constraint `regular` in your model. Running
```
picat feast.pi instance.pi
```
for the provided sample instance `instance.pi` should output the magnificence value of `33` and the sequence of dishes, one possibility is `[charsiubao,hotsoursoup,mapotofu,sesameprawn,kungpaochicken,coconutjelly]`.

(Adapted from Coursera course Basic modeling for discrete optimization.)
