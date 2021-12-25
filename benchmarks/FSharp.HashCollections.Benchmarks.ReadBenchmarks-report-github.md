``` ini

BenchmarkDotNet=v0.13.1, OS=arch 
AMD Ryzen 7 3700X, 1 CPU, 16 logical and 8 physical cores
.NET SDK=5.0.301
  [Host]     : .NET 5.0.7 (5.0.721.25508), X64 RyuJIT DEBUG
  DefaultJob : .NET 5.0.7 (5.0.721.25508), X64 RyuJIT


```
|                           Method | CollectionSize |        Mean |    Error |   StdDev |
|--------------------------------- |--------------- |------------:|---------:|---------:|
|                       **GetHashMap** |             **10** |    **11.27 ns** | **0.059 ns** | **0.052 ns** |
|                GetImToolsHashMap |             10 |    30.78 ns | 0.573 ns | 0.508 ns |
|                     GetFSharpMap |             10 |    38.90 ns | 0.535 ns | 0.474 ns |
|                GetFSharpXHashMap |             10 |    99.11 ns | 1.295 ns | 1.211 ns |
| GetSystemCollectionsImmutableMap |             10 |    22.65 ns | 0.201 ns | 0.178 ns |
|         GetFSharpDataAdaptiveMap |             10 |    21.06 ns | 0.187 ns | 0.175 ns |
|               GetFSharpxChampMap |             10 |    75.58 ns | 1.474 ns | 1.514 ns |
|                       **GetHashMap** |            **100** |    **15.27 ns** | **0.106 ns** | **0.099 ns** |
|                GetImToolsHashMap |            100 |    44.76 ns | 0.770 ns | 0.824 ns |
|                     GetFSharpMap |            100 |    70.82 ns | 0.638 ns | 0.565 ns |
|                GetFSharpXHashMap |            100 |   110.33 ns | 1.877 ns | 1.664 ns |
| GetSystemCollectionsImmutableMap |            100 |    34.41 ns | 0.377 ns | 0.353 ns |
|         GetFSharpDataAdaptiveMap |            100 |    42.18 ns | 0.533 ns | 0.499 ns |
|               GetFSharpxChampMap |            100 |    95.72 ns | 1.423 ns | 1.261 ns |
|                       **GetHashMap** |           **1000** |    **12.27 ns** | **0.086 ns** | **0.081 ns** |
|                GetImToolsHashMap |           1000 |    66.92 ns | 0.676 ns | 0.565 ns |
|                     GetFSharpMap |           1000 |   110.07 ns | 2.190 ns | 2.689 ns |
|                GetFSharpXHashMap |           1000 |   119.27 ns | 0.937 ns | 0.877 ns |
| GetSystemCollectionsImmutableMap |           1000 |    51.20 ns | 0.512 ns | 0.479 ns |
|         GetFSharpDataAdaptiveMap |           1000 |    65.18 ns | 0.827 ns | 0.773 ns |
|               GetFSharpxChampMap |           1000 |    96.31 ns | 1.018 ns | 0.902 ns |
|                       **GetHashMap** |         **100000** |    **27.10 ns** | **0.261 ns** | **0.244 ns** |
|                GetImToolsHashMap |         100000 |   192.91 ns | 1.385 ns | 1.295 ns |
|                     GetFSharpMap |         100000 |   202.18 ns | 3.977 ns | 3.720 ns |
|                GetFSharpXHashMap |         100000 |   142.92 ns | 1.867 ns | 1.655 ns |
| GetSystemCollectionsImmutableMap |         100000 |   143.54 ns | 1.211 ns | 1.133 ns |
|         GetFSharpDataAdaptiveMap |         100000 |   138.09 ns | 1.176 ns | 1.100 ns |
|               GetFSharpxChampMap |         100000 |   161.99 ns | 2.703 ns | 2.529 ns |
|                       **GetHashMap** |         **500000** |    **75.27 ns** | **0.464 ns** | **0.434 ns** |
|                GetImToolsHashMap |         500000 |   503.84 ns | 4.429 ns | 3.926 ns |
|                     GetFSharpMap |         500000 |   319.49 ns | 6.054 ns | 5.663 ns |
|                GetFSharpXHashMap |         500000 |   237.83 ns | 2.523 ns | 2.360 ns |
| GetSystemCollectionsImmutableMap |         500000 |   320.95 ns | 3.004 ns | 2.810 ns |
|         GetFSharpDataAdaptiveMap |         500000 |   303.34 ns | 2.013 ns | 1.883 ns |
|               GetFSharpxChampMap |         500000 |   169.03 ns | 1.864 ns | 1.744 ns |
|                       **GetHashMap** |         **750000** |   **108.07 ns** | **0.666 ns** | **0.623 ns** |
|                GetImToolsHashMap |         750000 |   608.60 ns | 3.202 ns | 2.838 ns |
|                     GetFSharpMap |         750000 |   406.83 ns | 4.744 ns | 4.437 ns |
|                GetFSharpXHashMap |         750000 |   351.69 ns | 1.921 ns | 1.797 ns |
| GetSystemCollectionsImmutableMap |         750000 |   409.93 ns | 2.075 ns | 1.941 ns |
|         GetFSharpDataAdaptiveMap |         750000 |   351.97 ns | 1.888 ns | 1.766 ns |
|               GetFSharpxChampMap |         750000 |   173.13 ns | 2.644 ns | 2.473 ns |
|                       **GetHashMap** |        **1000000** |   **114.22 ns** | **0.264 ns** | **0.247 ns** |
|                GetImToolsHashMap |        1000000 |   678.73 ns | 5.430 ns | 5.080 ns |
|                     GetFSharpMap |        1000000 |   472.68 ns | 3.494 ns | 3.097 ns |
|                GetFSharpXHashMap |        1000000 |   340.27 ns | 1.778 ns | 1.663 ns |
| GetSystemCollectionsImmutableMap |        1000000 |   468.81 ns | 4.030 ns | 3.770 ns |
|         GetFSharpDataAdaptiveMap |        1000000 |   392.71 ns | 2.035 ns | 1.903 ns |
|               GetFSharpxChampMap |        1000000 |   178.21 ns | 2.594 ns | 2.426 ns |
|                       **GetHashMap** |        **5000000** |   **146.63 ns** | **0.552 ns** | **0.516 ns** |
|                GetImToolsHashMap |        5000000 | 1,095.06 ns | 4.782 ns | 4.473 ns |
|                     GetFSharpMap |        5000000 |   803.83 ns | 4.079 ns | 3.816 ns |
|                GetFSharpXHashMap |        5000000 |   374.48 ns | 2.256 ns | 2.110 ns |
| GetSystemCollectionsImmutableMap |        5000000 |   775.52 ns | 5.161 ns | 4.828 ns |
|         GetFSharpDataAdaptiveMap |        5000000 |   556.44 ns | 2.809 ns | 2.628 ns |
|               GetFSharpxChampMap |        5000000 |   357.66 ns | 2.265 ns | 2.119 ns |
|                       **GetHashMap** |       **10000000** |   **163.68 ns** | **1.010 ns** | **0.944 ns** |
|                GetImToolsHashMap |       10000000 | 1,317.78 ns | 6.694 ns | 5.934 ns |
|                     GetFSharpMap |       10000000 |   935.86 ns | 4.086 ns | 3.822 ns |
|                GetFSharpXHashMap |       10000000 |   401.53 ns | 2.404 ns | 2.248 ns |
| GetSystemCollectionsImmutableMap |       10000000 |   909.51 ns | 2.906 ns | 2.576 ns |
|         GetFSharpDataAdaptiveMap |       10000000 |   655.68 ns | 2.443 ns | 2.040 ns |
|               GetFSharpxChampMap |       10000000 |   358.91 ns | 1.482 ns | 1.314 ns |