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

pointwise_threads: 1 row_block: 12 ht_transforms: 0 max_k: 128 max_nk: 32768 apf1: 1 bpf1: 1
        84.42,150.41,13.92 2.06,105.23,2.06 2.06,105.23,2.06  : 248.75 374.67 actual: 24.43,699.62,147.60 effective: 24.43,699.61,147.60 NEW BEST (374.67)
VGG 1.2 F(2x2,3x3): pointwise_threads: 1 row_block: 12 ht_transforms: 0 max_k: 128 max_nk: 32768 apf1: 1 bpf1: 1 ::: 374.672
