**Operaciones:**
- eq, exists, in, match, range, date range, geo_distance.
**Se pueden combinar con operadores:**
- and, or, not.
**Agregaciones:**
- terms, filter, histogram, avg, sum, min, max.
**Orden:**
- asc, desc.

```
{
  "size": 20,
  "query": {
    "eq": {
      "field": "STRING",
      "value": "(STRING|NUMBER)"
    }
  },
  "type": "query_and_fetch",
  "aggs": [
    {
      "name": "STRING",
      "field": "STRING",
      "type": "max"
    }
  ],
  "sort": [
    {
      "field": "last_indexed",
      "order": "asc"
    },
    {
      "field_type": "date"
    }
  ]
}
```