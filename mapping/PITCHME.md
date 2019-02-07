## Data strategy: Mapping service

---

## Mapping service

@ul[spaced-list-items]

* Replaces most lookups in allsports
* Centralizes all ids
  * External ids (e.g. opta, cricviz, pinnacle)
  * legacy internal ids (e.g. allsports, SD)
* One service used by all
* New smartodds Unique Id

@ulend

---

## Mapping Example

```javascript
{
    "entity_id" : 102347,
    "sport" : "cricket",
    "type" : "game",
    "lookups" : [
        {
            "source" : "cricket-quant",
            "external_id" : "853",
        },
        {
            "source" : "pinnacle",
            "external_id" : "45687",
        },
        {
            "source" : "cricviz",
            "external_id" : "172390",
        },
    ]
}
```
@[6-9](legacy internal source)
@[10-17](external sources)
@[2](Smartodds Unique Id)

---

## Phase 1: Mapping service integration

@ul[spaced-list-items]

* Integration of the mapping service in Allsports
* No change to the used Allsports data
* Minimal change to Allsports admin UI

@ulend

---

## Phase 2: Migration to Smartodds unique Id

@ul[spaced-list-items]

* Replacement of all reference to legacy ids by the corresponding Smartodds id
* No problems for models are calculated from scrach
* Migration needed for more persistent data e.g.
  * Stat Service
  * Cached data: Datashop Cache
  * QuantDBs

@ulend

---

## Feeback
Please amend the following document
https://confluence.smartodds.co.uk/display/~Nicolas.Leydet/Integration+of+the+mapping+service+and+its+impacts