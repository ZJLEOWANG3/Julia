I installed v1.6 previously, and now wanna remove it and install v1.7

1. In Julia, To find my Env for Julia 
```
ENV["PWD"]
```

2. In Terminal, Remove previous version for Julia
```
path = ENV["PWD"]
rm -rf path/compiled/v1.6
rm -rf path/environments/v1.6
```

3. In Julia, Add the kernel to Jupyter (will work for lab & notebook)
```
]
add IJulia
build IJulia
```

4. In Terminal, Remove previous version of Julia for Jupyter
```
jupyter kernelspec list
jupyter kernelspec uninstall julia-1.6
```
