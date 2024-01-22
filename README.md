# Welcome to Perlini
## What is it?
Perlini is a very simple, header-only, cross-platform static 2D Perlin-Noise generator.
## Installation
Simply add the Perlini.h header file to your project.
## Usage
```
/*
 *  Simple snippet to test Perlini
 */
#include <iostream>
#include "Perlini.h"                                            // include the header file

int main()
{
    Perlini::PerlinNoise2D::SetPrimeIndex(2);                   // sets the index of the primes to use (optional, default is 0)
    double val = Perlini::PerlinNoise2D::GetCoordValue(5, 4);   // gets the value at a certain 2D coordinate

    std::cout << val << std::endl;

    return 0;
}
