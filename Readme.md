# Reference-Guided Genome Assembler

This tool is a reference-guided genome assembler that utilizes the Burrows-Wheeler Transform (BWT) and Suffix Array for efficient genome assembly.

## Usage

Follow these steps to assemble your genome:

1. **Prepare Your Input Files**
   - Place your reads (one read per line) in a file named `reads.txt`.
   - Place your reference genome in a file named `genome.txt`.

2. **Compile the Code**
   - Run the following command to compile the source code with optimization:
     ```
     g++ -O3 main.cpp libsais.c libsais16.c libsais64.c
     ```

3. **Execute the Program**
   - After compilation, execute the program using:
     ```
     ./a.exe
     ```

4. **Output**
   - The assembled genome will be generated in a file named `assembled_genome.txt`.
   - This file will contain a contig per line, representing the assembled sequences.

Ensure that the input files `reads.txt` and `genome.txt` are correctly formatted and located in the same directory as the executable for the program to function properly.

## Credits and Acknowledgments

The **GenoWhisperers** team proudly developed this genome assembler. Team members include:

- Ali Baydoun
- Ali Saab
- Fatima Dekmak
- Hadi Al Khansa
- Raphael El Fakhri

We extend our sincere gratitude to Dr. Rida Assaf, our instructor who provided guidance and invaluable insights throughout the development process.

Special thanks to Ilya Grebnov for the `libsais` library, which is we used for BWT and suffix array construction. The library can be found at [libsais GitHub repository](https://github.com/IlyaGrebnov/libsais).
