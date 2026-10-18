# Cache Memory Mapping Simulator

**Name:** Atmika Hon
**PRN:** 2125UIDF1029
**Class:** SY CSE, Sanjivani University
**Subject:** Computer Organization and Architecture (COA), CO5 Micro Project

## About
This is a web-based simulator that shows how a CPU cache maps main memory
blocks to cache lines. It runs step by step so each memory access can be
followed: address split, tag comparison, hit or miss, and replacement.

## Features
- Three mapping techniques: direct mapped, fully associative, set associative
- Address split into tag, index and offset for every access
- Hit and miss display with colour coding
- Replacement policies: LRU and FIFO
- Adjustable parameters: address width, block size, cache lines, ways per set
- Custom address sequence in decimal or hex, or a random sequence
- Next, Previous, Run all and Reset controls
- Live cache table, access log, and hit and miss ratio

## How to run
Open `index.html` in any modern browser. No installation is needed.

## How it works
1. The address is split into tag, index and offset bits.
2. The index selects the set (direct mapping has one line per set, fully
   associative has a single set).
3. The tag is compared with every valid line in that set.
4. A match is a hit. Otherwise it is a miss, and the block is loaded from
   main memory into an empty line or replaces a victim line (LRU or FIFO).

## Tools used
HTML, CSS, JavaScript
