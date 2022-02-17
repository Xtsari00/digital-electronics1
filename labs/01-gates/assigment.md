# Lab 1: Bohdan Tsariuchenko

### De Morgan's laws



```vhdl
architecture dataflow of demorgan is
begin
    f_o      <= -- (not(b_i) and a_i) or (not(c_i) and not(b_i));
    f_nand_o <= -- (not(b_i) nand a_i) nand (not(c_i) nand not(b_i));
    f_nor_o  <= -- (b_i nor not(a_i)) or (c_i nor b_i);
end architecture dataflow;
```

3. Complete table with logic functions' values:

| **c** | **b** |**a** | **f(c,b,a)** | **f_NAND(c,b,a)** | **f_NOR(c,b,a)** |
| :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 | 1 | 1 |
| 0 | 0 | 1 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 |

### Distributive laws

1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!
![Screenshot 2022-02-17 at 11 40 28](https://user-images.githubusercontent.com/99403641/154459196-89a08cbf-f48a-465d-84c0-6e9e9106ff34.png)

   ![your figure]()

2. Link to your public EDA Playground example:

https://www.edaplayground.com/x/C5zC
