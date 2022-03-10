 **D-type FF**
   | **clk** | **d** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ↑ | 0 | 0 | 0 | q(n+1) has the same level as d |
   | ↑ | 0 | 1 | 0 | Output did not change |
   | ↑ | 1 | 0 | 1 | q(n+1) has the same level as d |
   | ↑ | 1 | 1 | 1 | Output did not change |

   **JK-type FF**
   | **clk** | **j** | **k** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-: | :-- |
   | ↑ | 0 | 0 | 0 | 0 | Output did not change |
   | ↑ | 0 | 0 | 1 | 1 | Output did not change |
   | ↑ | 0 | 1 | 0 | 0 | set output value |
   | ↑ | 0 | 1 | 1 | 0 | set output value |
   | ↑ | 1 | 0 | 0 | 1 | reset output value |
   | ↑ | 1 | 0 | 1 | 1 | reset output value |
   | ↑ | 1 | 1 | 0 | 1 | changes value of output signal |
   | ↑ | 1 | 1 | 1 | 0 | changes value of output signal |

   **T-type FF**
   | **clk** | **t** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ↑ | 0 | 0 | 0 | Output did not change |
   | ↑ | 0 | 1 | 1 | set output value |
   | ↑ | 1 | 0 | 1 | reset output value |
   | ↑ | 1 | 1 | 0 | changes value of output signal |

<a name="part1"></a>
