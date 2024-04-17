Extremely stripped down and simplified pipeline CPU with no cache. 

8 nibble Instruction RAM, 2 nibble Data Ram, 2 nibble Register Block, all data is in nibbles. 

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


