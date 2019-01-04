# API Document

## Launch API Server

```
$ cd api-server
$ bundle install
$ bundle exec foreman start
$ open http://localhost:5000
```

## GET /items

### Response

```
{
  "data": [
    {
      "id": "1",
      "name": "men1",
      "description": "size free 1",
      "like_count": 91,
      "comment_count": 59,
      "price": 51,
      "isSoldOut": false,
      "shippingFee": "23",
      "image": "http://dummyimage.com/400x400/000/fff?text=men1"
    },
    {
      "id": "2",
      "name": "men2",
      "description": "size free 1",
      "like_count": 0,
      "comment_count": 0,
      "price": 10000,
      "isSoldOut": true,
      "shippingFee": "13",
      "image": "http://dummyimage.com/400x400/000/fff?text=men2"
    },
    ...
  ]
}
```

## GET /items/:id

### Response

```
{
  {
    "id": "1",
    "name": "men1",
    "description": "size free 1",
    "like_count": 91,
    "comment_count": 59,
    "price": 51,
    "isSoldOut": false,
    "shippingFee": "11",
    "image": "http://dummyimage.com/400x400/000/fff?text=men1"
  }
}
```

## GET /categories

### Response

```
{
  "data": [
    {
      "id": "1",
      "name": "test 1"
    },
    {
      "id": "2",
      "name": "test 2"
    },
    {
      "id": "3",
      "name": "test 3"
    },
    {
      "id": "4",
      "name": "test 4"
    },
    {
      "id": "5",
      "name": "test 5"
    }
  ]
}
```
