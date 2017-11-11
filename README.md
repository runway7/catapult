# Catapult

### `POST /bucket/key?token=abcd1234`

With Content-Type header and data in body. 

Return 
```
{
  "bucket": "b1",
  "key": "k1"
  "version": "v1"
}
```

### `GET /bucket/key/version`

Data returned with Content Type.

### `GET /bucket/key -> 302 Found to /bucket/key/latest_version`

### `DELETE /bucket/key?token=abcd1234`
