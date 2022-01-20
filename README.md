# Worklog2021Summer
#### Newest update
##### 20220108
Finished correctness check of input_transform, output_transform, filter_transform, results up to before pointwise correct. Pointwise gemm output might be at wrong address.
##### 20220113
Get the program runnable with acceptable accuracy
##### 20220118
Move project to m6g-metal machine so that it can run on 64-core-cpu with maximized performance.
##### 20220120
Performance: 

pointwise_threads: 2 row_block: 12 ht_transforms: 0 max_k: 128 max_nk: 16384 apf1: 1 bpf1: 1
        84.38,4860.96,13.83 2.06,105.23,2.06 2.06,105.23,2.06  : 4959.17 5085.05 actual: 24.45,21.65,148.59 effective: 24.45,21.65,148.59 NEW BEST (5085.05)
VGG 1.2 F(2x2,3x3): pointwise_threads: 2 row_block: 12 ht_transforms: 0 max_k: 128 max_nk: 16384 apf1: 1 bpf1: 1 ::: 5085.05
