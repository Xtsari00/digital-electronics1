# Lab 6: Bohdan Tsariuchenko 

### Bidirectional counter

1. Listing of VHDL code of the completed process `p_cnt_up_down`. Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

```vhdl
    --------------------------------------------------------
    -- p_cnt_up_down:
    -- Clocked process with synchronous reset which implements
    -- n-bit up/down counter.
    --------------------------------------------------------
    p_cnt_up_down : process(clk)
    begin
        if rising_edge(clk) then
        
            if (reset = '1') then   -- Synchronous reset
                s_cnt_local <= (others => '0'); -- Clear all bits

            elsif (en_i = '1') then -- Test if counter is enabled

                -- TEST COUNTER DIRECTION HERE
                    if (cnt_up_i = '1') then
                    s_cnt_local <= s_cnt_local + 1;
                    elsif (cnt_up_i ='0') then
                    s_cnt_local <= s_cnt_local - 1;
                    end if;
            end if;
        end if;
    end process p_cnt_up_down;
```

2. Screenshot with simulated time waveforms. Test reset as well. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

Reset 
![image](https://user-images.githubusercontent.com/99403641/159755616-c23a3943-6535-4c2f-979d-140ff3fea094.png)

Counting down 
![image](https://user-images.githubusercontent.com/99403641/159755664-5e4c4fbe-062b-4015-9c0e-351ce5fc5332.png)

Enable
![image](https://user-images.githubusercontent.com/99403641/159755714-9b617bd5-9304-4524-82ff-b6a243693acf.png)

### Two counters

1. Image of the top layer structure including both counters, ie a 4-bit bidirectional counter from *Part 4* and a 16-bit counter with a 10 ms time base from *Experiments on your own*. The image can be drawn on a computer or by hand. Always name all inputs, outputs, components and internal signals!

   
  IMG_4250.HEIC![image](https://user-images.githubusercontent.com/99403641/159764601-e14a2d69-3428-4862-8eb5-af9aa49030d9.png)


