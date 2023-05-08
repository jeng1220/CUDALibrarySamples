#  Mixed Precision GEMM (in:BF16, out:FP32) example #

## Build ##
```sh
cd <your path>/CUDALibrarySamples/cuBLASLt
mkdir build
cd build
make -j`nproc`
```

## Run ##
```sh
# build
nsys profile -t cuda --gpu-metrics-device all --stats true ./LtSgemm/sample_cublasLt_LtSgemm
```
See `SM Instructions/Tensor Active` in nsys.