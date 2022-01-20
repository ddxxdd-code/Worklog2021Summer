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

[DONE] Bench of layerVGG 1.2 F(2x2,3x3): 64 64 16 1 226 226  M_SIZE: 1,2,2 K_SIZE: 1,3,3

[BEST] for VGG 1.2 F(2x2,3x3) is 184.285
[BEST] VGG 1.2 F(2x2,3x3) :: pointwise_threads: 1 row_block: 26 ht_transforms: 0 max_k: 128 max_nk: 16384 apf1: 1 bpf1: 1 ms
