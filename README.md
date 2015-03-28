# United States National Park Service Parks, Recreation Areas, Forests, Preserve, Historic Sites, Historic Trails, River Corridors, and Monuments

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
  {TypeName}: [TerritoryObject]
}
```

#### TerritoryObject Shape

```json
{
  "name": String,
  "location": LocationObject,
  "area": String,
  "length": String,
  "recreation: RecreationObject,
  "website": String
}
```

#### LocationObject Shape

```json
{
  "territory": [String],
  "state": [String],
  "city": [String],
  "coordinates": {

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
$ npm test
$ npm run build
```

### Build Input

* `./data/{type}/{name}.hjson`

### Build Output

* `./data/{type}.json`
* `./data.json`
