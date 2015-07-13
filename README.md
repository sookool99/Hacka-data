# Hacka-data
Get Data for all your hackathon needs

## Getting started

update dependancies `npm i`

You Must have a `.yelp_credentials` with the following information:
```
{
    "consumer_key": "your_key",
    "consumer_secret": "your_secret",
    "token": "your_token",
    "token_secret": "your_token_secret"
}
```

### To run script:
```
node run.js "Location" [categories]
```
Where location is the area in which you want results, places with more then one name, such as Halifax, you will need to also supply state/province code along with it to specifiy which one you want. example: "Halifax, NS".

The categories is just n number of categories you want to search by, seporated by a space (example with more then one category below)

#### Examples

If you want to get just one of the categories then, lets say just vet:
```
node run.js "halifax, NS" vet
```

you can group the search by different categories, lets say you want to group all vets who also have dogwalking services.
```
node run.js "Halifax, NS" vet dogwalkers
```

## List of categorys
```
https://www.yelp.com/developers/documentation/v2/all_category_list
```

