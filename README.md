# profiler to see

https://github.com/zhijian-liu/torchprofile

# profilerForLLM_HuggingFace

Files:
1. llamaModelProfiler.py
2. llamaModelrofilerWithOutput.py
3. profilerWithJsonStorage.py


**Calculate flops and memory requirements for each layer, Given sequence length and Max Tokens.**

##### To run script
```bash
python llamaModelProfiler.py
```

##### Output will seems to be

```bash
Layer                Inference FLOPs      Memory (MB)    
-------------------------------------------------------
Embedding            2,048,000            250.00         
Layer 0              226,673,590          386.02         
Layer 1              226,673,590          386.02         
Layer 2              226,673,590          386.02         
Layer 3              226,673,590          386.02         
Layer 4              226,673,590          386.02         
Layer 5              226,673,590          386.02         
Layer 6              226,673,590          386.02         
Layer 7              226,673,590          386.02         
Layer 8              226,673,590          386.02         
Layer 9              226,673,590          386.02         
Layer 10             226,673,590          386.02         
Layer 11             226,673,590          386.02         
Layer 12             226,673,590          386.02         
Layer 13             226,673,590          386.02         
Layer 14             226,673,590          386.02         
Layer 15             226,673,590          386.02         
Layer 16             226,673,590          386.02         
Layer 17             226,673,590          386.02         
Layer 18             226,673,590          386.02         
Layer 19             226,673,590          386.02         
Layer 20             226,673,590          386.02         
Layer 21             226,673,590          386.02         
Layer 22             226,673,590          386.02         
Layer 23             226,673,590          386.02         
Layer 24             226,673,590          386.02         
Layer 25             226,673,590          386.02         
Layer 26             226,673,590          386.02         
Layer 27             226,673,590          386.02         
Layer 28             226,673,590          386.02         
Layer 29             226,673,590          386.02         
Layer 30             226,673,590          386.02         
Layer 31             226,673,590          386.02         
Final LayerNorm      229,376              0.01           
-------------------------------------------------------
Total                7,255,832,246        12602.51       

Total Inference FLOPs for 28 new tokens: 7,255,832,246
Total Memory Usage: 12602.51 MB
```

**To get output of each layer**

##### To run script
```bash
python llamaModelProfilerWithOutput.py
```
##### Output 
```bash
Layer                Inference FLOPs      Memory (MB)     Output Size    
----------------------------------------------------------------------
Embedding            40,960               1002.00         (10, 4096)
Layer 0              6,328,422,646        416.02          (10, 4096)
Layer 1              6,328,422,646        416.02          (10, 4096)
Layer 2              6,328,422,646        416.02          (10, 4096)
Layer 3              6,328,422,646        416.02          (10, 4096)
Layer 4              6,328,422,646        416.02          (10, 4096)
Layer 5              6,328,422,646        416.02          (10, 4096)
Layer 6              6,328,422,646        416.02          (10, 4096)
Layer 7              6,328,422,646        416.02          (10, 4096)
Layer 8              6,328,422,646        416.02          (10, 4096)
Layer 9              6,328,422,646        416.02          (10, 4096)
Layer 10             6,328,422,646        416.02          (10, 4096)
Layer 11             6,328,422,646        416.02          (10, 4096)
Layer 12             6,328,422,646        416.02          (10, 4096)
Layer 13             6,328,422,646        416.02          (10, 4096)
Layer 14             6,328,422,646        416.02          (10, 4096)
Layer 15             6,328,422,646        416.02          (10, 4096)
Layer 16             6,328,422,646        416.02          (10, 4096)
Layer 17             6,328,422,646        416.02          (10, 4096)
Layer 18             6,328,422,646        416.02          (10, 4096)
Layer 19             6,328,422,646        416.02          (10, 4096)
Layer 20             6,328,422,646        416.02          (10, 4096)
Layer 21             6,328,422,646        416.02          (10, 4096)
Layer 22             6,328,422,646        416.02          (10, 4096)
Layer 23             6,328,422,646        416.02          (10, 4096)
Layer 24             6,328,422,646        416.02          (10, 4096)
Layer 25             6,328,422,646        416.02          (10, 4096)
Layer 26             6,328,422,646        416.02          (10, 4096)
Layer 27             6,328,422,646        416.02          (10, 4096)
Layer 28             6,328,422,646        416.02          (10, 4096)
Layer 29             6,328,422,646        416.02          (10, 4096)
Layer 30             6,328,422,646        416.02          (10, 4096)
Layer 31             6,328,422,646        416.02          (10, 4096)
Final LayerNorm      2,048,000            0.01            (10, 4096)
----------------------------------------------------------------------
Total                202,511,613,646      14314.51       

Total Inference FLOPs for 250 new tokens: 202,511,613,646
Total Memory Usage: 14314.51 MB
```















