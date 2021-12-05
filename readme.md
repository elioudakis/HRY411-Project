Semester project - Sudoku on Atmel AVR
Course               : HRY411 - Embedded Microprocessor Systems, Winter Semester of acad. year 2021-22
Students             : Kallinteris Andreas, 2017030066
                     : Lioudakis Emmanouil, 2018030020
Device in simulation : ATmega16 (WARNING: If another device is used, some registers may differ a bit)
Device in STK500     : ATmega16L - fully compatible with ATmega16
IDE used             : Microchip Studio 7
CPU freq             : 10 MHz, using an oscillator in STK500 (If changed, things such as timer init. value and UBRR for the serial port should change too)

# build instructions

## using gnu-toolchain on linux

```
git clone https://github.com/apcountryman/toolchain-avr-gcc.git
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=../toolchain-avr-gcc/toolchain.cmake -DCMAKE_BUILD_TYPE=RelWithDebInfo .. && make
```



## using microchip studio

make sure to use gnu c++ compiler (g++) and provide the flags `-DAVR --std=c++17`
