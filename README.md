# VSO-1587059

To test:

```
> git submodule update --init vcpkg
> cmake -B build -S . -G Ninja
> cmake --build build
```
