Extremely stripped down and simplified pipeline CPU with no cache. 8 nibble Instruction RAM, 2 nibble Data Ram, 2 nibble Register Block, all data is in nibbles. 

4 possible instructions: ADD, SUB, LOAD, SUB. 

Opcode structure is 4 bits: `____`

first 2 bits are the instruction. 
- `00__` LOAD
- `01__` SAVE
- `10__` ADD
- `11__` SUB

3rd bit is the register
- `__0_` for $r0
- `__1_` for $r1

4th bit is the Data RAM
- `___0` for ram address 0
- `___1` for ram address 1
