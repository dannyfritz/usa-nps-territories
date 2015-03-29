# United States National Park Service Parks, Recreation Areas, Forests, Preserves, Historic Sites, Historic Trails, River Corridors, and Monuments

This is an unofficial repository containing information about
the various NPS territories in the United States of America.

## Unofficial

I am not affliated with the National Parks Service or the
federal government.

I just like parks and nature. :evergreen_tree: :mount_fuji: :deciduous_tree: :smile:

## data.json

### Shape

```json
{
  "data": [TerritoryObject]
}
```

#### TerritoryObject Shape

```json
{
  "name": String,
  "type": String or [String],
  "location": LocationObject or [LocationObject],
  "area": String,
  "length": String,
  "recreation": RecreationObject,
  "slug": String,
  "website": String
}
```

#### LocationObject Shape

```json
{
  "territory": String,
  "state": String,
  "county": String,
  "city": String,
  "coordinates": {
      //TODO
  }
}
```

#### RecreationObject Shape

```json
{
  "campgrounds": Boolean,
  "dispersedCamping": Boolean,
  "hiking": Boolean
}
```

## Build

```bash
$ npm install
$ npm run build
```

### Build Input

* `./data/*.hjson`

### Build Output

* `./data/{type}.json`
* `./data.json`
