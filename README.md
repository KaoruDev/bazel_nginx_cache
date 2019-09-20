# Bazel Remote Cache with nginx inside of Docker
So many buzzwords...


## Building

```
docker build -t bazel_cache:0.0.1 .
```


## Running

```
docker run -it --rm --name=bazelcache \
  -p3232:3232
  -v path/to/local/cache_dir:/data/bazel/cache \
  bazel_cache:0.0.1
```
