* basics

```
> db
test

> show dbs
admin  (empty)
test   0.078GB

> use test
switched to db test

> show collections
>
```

* insert

```
> db.mycoll.insert({a:1})
```

* update

```
> db.mycoll.update(
... { _id:ObjectId("54759d9c212ff46df7bd7b53") },
... { $set: {a:2, b:{aa:1} } }
... )
```

* delete

```
> db.mycoll.remove( { _id: ObjectId("54759d9c212ff46df7bd7b53") } )
WriteResult({ "nRemoved" : 1 })
```

* find

```
> db.mycoll.find()
> db.mycoll.find().pretty()
```
