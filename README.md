# delicia-model

This a repository of a noSQL database nmodel design of 'Delicia', a food ordering app.

<hr>
There are four collections in this model:

- `items.json:` consists of normalized data model of the food items to be sold. Here, the `reveiwId` field of collection `items_review.json` was refrenced.
- `customers.json:` consists of denormalized data model of the registered customers.
- `orders.json:` consists of denormalized data model of the ordered items.
- `items_review.json:` Here, the `itemId` & `customerId` field of collection `items.json` & `customers.json` were refrenced.
<hr>

> Performance was considered while designing `items.json` & `items_review.json` hence, the adoption of normalaized (refrence) design model.
> Consistency and query pattern was considered while designing `customers.json:` & `items_review.json:` hence, the adoption of denormalized (embeded) data model.
