# WeberCedrus

This Julia package extends [Weber](https://github.com/haberdashPI/Weber.jl), to enable the use of Cedrus response-pad input. It adds a series of new keys, ranging from key":cedrus0:" to key":cedrus19:'. You can see which key is which by pressing the buttons while running the following code in julia.

```julia
using Weber
using WeberCedrus
run_keycode_helper(extenstions=[Cedrus()])
```

To make use of the response keys, just reference them as you would keyboard
keys. For instance, the following would record cedrus buttons 1 and 2
ans answer 1 and 2, in the experiment data file.

```julia
response(key":cedrus1:" => "answer1", key":cedrus2:" => "answer2")
```




