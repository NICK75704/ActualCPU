| Mini Instruction             | Shortcut Term               | PLA Place |
| ---------------------------- | --------------------------- | --------- |
| read next byte               | RNB (read next byte)        | 0         |
| read address to jump to      | RAJ (read address jump)     | 1         |
| store current address to RAM | SAS (store address stack)   | 2         |
| jump to address              | JPA (jump address)          | 3         |
| read from address            | RDA (read address)          | 4         |
| load to A                    | LTA (load to A)             | 5         |
| load to B                    | LTB (load to B)             | 6         |
| return from address          | RFA (return from address)   | 7         |
| store A to bus               | SAB                         | 8         |
| store B to bus               | SBB                         | 9         |
| compare A and B              | CAB (compare A B)           | 10        |
| RAM write enable             | RWE (ram write enable)      | 11        |
| RAM write disable            | RWD (ram write disable)     | 12        |
|                              |                             |           |
|                              |                             |           |
| move to next instruction     | MNI (move next instruction) | 15        |



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



