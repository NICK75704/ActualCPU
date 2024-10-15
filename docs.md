| Mini Instruction             | Shortcut Term               |
| ---------------------------- | --------------------------- |
| read address to jump to      | RAJ (read address jump)     |
| store current address to RAM | SAS (store address stack)   |
| jump to address              | JPA (jump address)          |
| read from address            | RDA (read address)          |
| return from address          | RFA (return from address)   |
| read next byte               | RNB (read next byte)        |
| load to A                    | LTA (load to A)             |
| store A to bus               | SAB                         |
| load to B                    | LTB (load to B)             |
| store B to bus               | SBB                         |
| compare A and B              | CAB (compare A B)           |
| move to next instruction     | MNI (move next instruction) |
| RAM write enable             | RWE (ram write enable)      |
| RAM write disable            | RWD (ram write disable)     |



| Instruction               | Operations                                  | Label    |
| ------------------------- | ------------------------------------------- | -------- |
| load a from address       | RAJ, RWE, SAS, RWD, JPA, RDA, LTA, RFA, MNI | 1 (01)   |
| load a from integer       | RNB, LTA, MNI                               | 2 (10)   |
| load b from address       | RAJ, RWE. SAS, RWD, JPA, RDA, LTB, RFA, MNI | 3 (11)   |
| load b from intager       | RNB, LTB, MNI                               | 4 (100)  |
| store a to address        | RAJ, RWE, SAS, RWD, JPA, SAB, RFA, MNI      | 5 (101)  |
| store b to address        | RAJ, RWE, SAS, RWD, JPA, SBB, RFA, MNI      | 6 (110)  |
| jump                      |                                             | 7 (111)  |
| jump if a and b are equal |                                             | 8 (1000) |



| Memory Location | Allocation |
| --------------- | ---------- |
| 0-63            | ROM        |
| 64-127          | RAM        |
| 128-256         | I/O        |



