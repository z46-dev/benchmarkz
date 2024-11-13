# Benchmarkz

This project aims to better benchmark many languages I work with in ways I actually care about. Number crunching isn't everything, and therefore we should have better data.
The benchmarking engine is written in Go, and will check against the following languages, along with certain revisions for each one.

## Languages

- C
    - GCC
    - Clang
- C++
- Java
- Go
- Rust
- JavaScript
    - Node
    - Deno
    - Bun
- Scala

Please make sure you have the tools to run everything above for best results. If you don't, a test will be skipped.

## Tests

- Math
    - Prime numbers
    - Hashing algorithms (brute force proof of work)
- HTTP Server
    - Requests/sec
    - Requests/sec with size
- File I/O
    - Reading and writing large files
    - Open/Close speeds
- String manipulation
    - Tokenize a large file
- Concurrency
    - Simple map-reduce algorithm
    - Data sharing (GB/s)

## Methodology of Testing

Some of these tests can be run concurrently quite nicely using Go, others can not. For better results, concurrency can be 