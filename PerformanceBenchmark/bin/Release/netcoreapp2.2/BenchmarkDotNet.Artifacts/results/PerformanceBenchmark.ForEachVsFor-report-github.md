``` ini

BenchmarkDotNet=v0.11.5, OS=Windows 10.0.17134.829 (1803/April2018Update/Redstone4)
Intel Core i7-6600U CPU 2.60GHz (Skylake), 1 CPU, 4 logical and 2 physical cores
Frequency=2742189 Hz, Resolution=364.6722 ns, Timer=TSC
.NET Core SDK=2.2.401
  [Host] : .NET Core 2.2.6 (CoreCLR 4.6.27817.03, CoreFX 4.6.27818.02), 64bit RyuJIT  [AttachedDebugger]
  Core   : .NET Core 2.2.6 (CoreCLR 4.6.27817.03, CoreFX 4.6.27818.02), 64bit RyuJIT

Job=Core  Runtime=Core  

```
|        Method |    N |          Mean |        Error |        StdDev |        Median | Ratio | Rank |
|-------------- |----- |--------------:|-------------:|--------------:|--------------:|------:|-----:|
| **StringBuilder** |   **10** |      **61.00 ns** |     **2.517 ns** |      **7.302 ns** |      **56.76 ns** |  **1.00** |    **1** |
|               |      |               |              |               |               |       |      |
|        String |   10 |     272.35 ns |    15.206 ns |     44.358 ns |     263.45 ns |  1.00 |    1 |
|               |      |               |              |               |               |       |      |
| **StringBuilder** |  **100** |     **677.29 ns** |    **30.566 ns** |     **89.645 ns** |     **681.18 ns** |  **1.00** |    **1** |
|               |      |               |              |               |               |       |      |
|        String |  100 |   3,178.52 ns |   166.469 ns |    490.839 ns |   3,116.52 ns |  1.00 |    1 |
|               |      |               |              |               |               |       |      |
| **StringBuilder** | **1000** |   **5,045.98 ns** |   **260.866 ns** |    **769.170 ns** |   **5,015.87 ns** |  **1.00** |    **1** |
|               |      |               |              |               |               |       |      |
|        String | 1000 | 139,942.63 ns | 6,179.831 ns | 18,221.372 ns | 137,344.88 ns |  1.00 |    1 |
