![image](https://github.com/rayane-b/comp273-final-project/assets/44729925/9875dc51-aec1-449e-877f-0d91b36f666f)

Extremely stripped down and simplified pipeline CPU with no cache. 

Load data into the Data RAM, load your instructions into the Instruction RAM and start the clock.

8 nibble Instruction RAM, 2 nibble Data RAM, 2 nibble Register Block, all data is in nibbles. 

Opcode is 1 nibble: `_ _ _ _`

- first 2 bits are the instruction: ADD, SUB, LOAD, SUB, HALT
  - `00__` LOAD 
  - `01__` SAVE 
  - `10__` ADD 
  - `11__` SUB 
  - `1111` reserved for HALT

- 3rd bit is the register
    - `0` for $r0
    - `1` for $r1  
- 4th bit is the Data RAM address
  - `0` for ram address 0
  - `1` for ram address 1 



