# zsvlib
 Zero runtime-allocation csv handling library in Zig

## use cases
- use case 1: tool to compute+dump typed description for necessary file sizes
- use case 2: tool to compute+dump typed description for necessary memory sizes
- use case 2: tool to combine multiple typed descriptions for necessary memory sizes
- use case 3: comptime layout generation for memory per csv line or whole file
- use case 4: library to use optionally SIMD for parsing data
- use case 5: library to write data to schemas.
* Opt-in of allocations with size must be possible.
- non-goal(for now): csv variations compatibility.
- non-goal: support fancy or many types
- non-goal: conversion to other formats
- non-goal: dealing with other string encoding than ascii and utf8
- non-goal: interaction besides the csv header generation
- non-goal(for now): updating offset to peek and write to file positions

## planned interfaces
todo

## status
wip.

## todos
- [ ] prototype csv parsing
- [ ] zig build
- [ ] describe how files are encoded (types + file sizes)
- [ ] describe how memory layouts are encoded (types + file sizes)
- [ ] describe how memory layouts are read at comptime (types + file sizes)
- [ ] implement how files are encoded (types + file sizes)
- [ ] implement how memory layouts are encoded (types + file sizes)
- [ ] implement how memory layouts are read at comptime (types + file sizes)
- [ ] tests headergen
- [ ] tests header reading
- [ ] tests codegen from header
- [ ] perf headergen
- [ ] perf header reading
- [ ] perf codegen from header
- [ ] simd csv parsing
- [ ] perf simd

## obsoletion plan
no plan for obsolation

## notes

https://nullprogram.com/blog/2021/12/04/
bit hacks for perf
https://wunkolo.github.io/post/2020/05/pclmulqdq-tricks/
https://github.com/geofflangdale/simdcsv
https://github.com/dbro/csvquote
"Speculative Distributed CSV Data Parsing for Big Data Analytics" by Ge et al.
https://www.microsoft.com/en-us/research/publication/speculative-distributed-csv-data-parsing-for-big-data-analytics/
"Instant Loading for Main Memory Databases" by Mühlbauar et al.
https://www.semanticscholar.org/paper/Instant-Loading-for-Main-Memory-Databases-M%C3%BChlbauer-R%C3%B6diger/a1b067fc941d6727169ec18a882080fa1f074595?p2df
