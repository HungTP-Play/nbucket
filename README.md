# nbucket

![Logo](nbucket.png)

`nbucket` is a simple easy to use for rate limiting requests or throttling requests.

`nbucket` can be used with any web framework or any other application, like: Gin, Fiber, Echo, Iris, etc.

`nbucket` by default, it will use local memory to store the buckets, but you can use Redis or Memcached to store the buckets or other `storage driver` that you want.

We have built-in `storage drivers` for `local driver`, `redis driver`, `memcached driver`,and `keydb driver`. You can also create your own `storage driver` by implementing the `StorageDriver` interface.

`nbucket` is policy based, you can create multiple policies with different configurations.

We also have built-in `limiter` and `throttler` policies, you can also create your own policy by implementing the `Policy` interface.

## Requirements

- Go 1.19 or higher
