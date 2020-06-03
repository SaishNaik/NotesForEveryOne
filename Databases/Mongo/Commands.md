#Commands

Mongo export with query to write to a file

```mongoexport -u user -p pwd --authenticationDatabase ad --db db -c collection -q '{ "x": 1,"y":{$gte:2},"y":{$lte:4}}' --out out.json```

Mongo import with the above mentioned export
```mongoimport --db db --collection collection --file out.json```
