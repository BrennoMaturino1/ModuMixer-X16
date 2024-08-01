# ModuMixer X16
ModuMixer is a modular digital audio mixer project with an almost unlimited amount of input and output channels (the limit is 65536)
It can be customized with input or output modules that are recognized by the "main computer"
The cue and main output signals are connected together in a summing amplifier configuration where each module sums it's signal to the data lines
The modules are digitally recognized by a custom protocol over USART where during boot one module is powered at a time and receives an address from the main computer (i know connecting multiple devices to USART isn't a good idea but i guess it will work), the digital signal processing works with an STM32 microcontroller for processing and a codec for digital to analog and analog to digital conversions
