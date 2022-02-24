# Lab 2: Bohdan Tsariuchenko

### 2-bit comparator

1. Karnaugh maps for other two functions:

   Greater than:

   ![image](https://user-images.githubusercontent.com/99403641/155399414-9c2dc72f-9086-4122-b1ba-02cf7aab797e.png)


   Less than:

   ![image](https://user-images.githubusercontent.com/99403641/155399440-a744c78a-3798-4377-9851-b3bfde898058.png)


2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

  ![image](https://user-images.githubusercontent.com/99403641/155403283-59ab138c-be41-4e9c-a476-4a9670413975.png)


### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

   Last two digits of my student ID: 230334

```vhdl
    p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
        report "Stimulus process started" severity note;

        -- First test case
        s_b <= "0011"; --3
        s_a <= "0100"; --4
        wait for 100 ns;
        -- Expected output
        assert ((s_B_greater_A = '0') and
                (s_B_equals_A  = '0') and
                (s_B_less_A    = '1'))
        -- If false, then report an error
        report "Input combination COMPLETE_THIS_TEXT FAILED" severity error;

        -- Report a note at the end of stimulus process
        report "Stimulus process finished" severity note;
        wait;
    end process p_stimulus;
```

2. Text console screenshot during your simulation, including reports.

   ![image](https://user-images.githubusercontent.com/99403641/155475242-789dbb42-e63d-426c-9ab4-42e94e80f0f4.png)


3. Link to your public EDA Playground example:

   https://www.edaplayground.com/x/dfu6
