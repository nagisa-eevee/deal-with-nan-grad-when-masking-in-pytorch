# deal-with-nan-grad-when-masking-in-pytorch
I got nan grad when backward a piecewise function in pytorch, 
and the function uses a mask(something like `mask = x > threshold`) to split input `x` into several intervals.

I found two ways to deal with it, both using **hook** or **build-in functions** instead of masking. 
Both of them have some drawbacks, and I want to find a simple & universal way to deal with it.
