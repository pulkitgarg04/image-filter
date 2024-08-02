# Image Filter
This project provides a command-line tool for applying various image filters to bitmap images. The tool supports grayscale, sepia, reflection, and blur effects.

### Requirements
**Compiler**: gcc or clang (for compiling the source code)

### Compilation
To compile the source code, use the following command:

For gcc:
```shell
gcc -ggdb3 -gdwarf-4 -O0 -std=c11 -Wall -Werror -Wextra -Wno-gnu-folding-constant -Wno-sign-compare -Wno-unused-parameter -Wno-unused-variable -Wshadow -lm -o filter filter.c helpers.c
```
For clang:
```shell
clang -ggdb3 -gdwarf-4 -O0 -std=c11 -Wall -Werror -Wextra -Wno-gnu-folding-constant -Wno-sign-compare -Wno-unused-parameter -Wno-unused-variable -Wshadow -lm -o filter filter.c helpers.c
```

This command will generate an executable named filter.

### Usage
You can apply different filters to your images using the following commands:

**Grayscale**:
Convert an image to grayscale:
```shell
./filter -g ./images/courtyard.bmp ./images/courtyard-grayscale.bmp
```

**Sepia**:
Apply a sepia tone to an image:
```shell
./filter -s ./images/stadium.bmp ./images/stadium-sepia.bmp
```

**Reflection**:
Create a horizontally reflected version of an image:
```shell
./filter -r ./images/tower.bmp ./images/tower-reflected.bmp
```

**Blur**:
Apply a blur effect to an image:
```shell
./filter -b ./images/yard.bmp ./images/yard-blurred.bmp
```

### Parameters
-g: Apply grayscale filter
-s: Apply sepia filter
-r: Apply reflection filter
-b: Apply blur filter

### Image Paths
Ensure that the input image files are located in the ./images/ directory and that the output paths specified are correct.