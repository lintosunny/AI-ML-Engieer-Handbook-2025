# Unit 1: Digital Information
## Binary system
Computer represent data using binary data, 1s and 0s.<br>
For images each pixel will get 3 values and using this color can be sorted.<br>
A bit is the smallest piece of information in a computer, a single value storing either 0 or 1.<br>
A byte is a unit of digital information that consists of 8 of those bits.

Decimal number system uses ..., 1000s, 100s, 10s, 1s but binary system uses ..., 8, 4, 2, 1 ( ..., 2<sup>3</sup>, 2<sup>2</sup>, 2<sup>1</sup>, 2<sup>0</sup>) <br>
Decimal system: 229 -> 100x2 + 10x2 + 1x9 <br>
Binary system: 1 0 0 1 -> 1x8 + 0x4 + 0x2 + 1x1 -> 9 

## Limitation of storing numbers
An integer is any number that can be written without a fractional component.<br>
If computer uses 4 bits to represent integers, then 7 will be represented like this: 0 1 1 1 -> +/- 4 2 1<br>
First bit represents it's a positive or negative number. 0 for +ve and 1 for -ve.<br>

**Overflow** is we are using a 4 bits computer and want to represent 8. But it is not possible because 7 is the largest integer it can represent with the 4 bits. In this case computer might report an "overflow error" or display "number is too large".

floating-point representation for non-integers (also integers if needed)<br>
Once the computer determines the floating point representation for a number, it stores that in bits. Modern computers use a 64-bit system that uses 1 bit for the sign, 11 bits for the exponent, and 52 bits for the number in front.<br>
160 = 1.25 x 2<sup>7</sup> <br>
0.50 = 1 x 2<sup>-1</sup> <br>
0.375 = 1.5 x 2<sup>-2</sup> -> 0011111111011000000000000000000000000000000000000000000000000000

This can't fully represent all numbers. Numbers like 1/3 is an infinitely repeating sequence. 1/10 (which is short in decimal 0.1) end up as infinitely repeating sequences once converted to binary. We often don't notice the lower precision of a number's representation until we use it in calculations. That's when we can experience a **roundoff error** in the results.

## Compression
compression algorithms to reduce the amount of space needed to represent a file. There are two types of compression: lossless and lossy.

Lossless compression algorithms reduce the size of files without losing any information in the file, which means that we can reconstruct the original data from the compressed file.
* Lossless text compression -> Compression algorithm
* Lossless image compression -> Run-Length Encoding (RLE)
* Lossless bit compression -> Huffman coding algorithm

Lossy compression algorithms reduce the size of files by discarding the less important information in a file, which can significantly reduce file size but also affect file quality.

# Unit 2: The Internet
The Internet is a global network of computing devices communicating with each other in some way, whether they're sending emails, downloading files, or sharing websites. It is an open network and rules are known as **protocols.** To create a global network of computing devices, we need: 
* Wires & wireless: Physical connections between devices, plus protocols for converting electromagnetic signals into binary data.
* IP: A protocol that uniquely identify devices using IP addresses and provides a routing strategy to send data to a destination IP address.
* TCP/UDP: Protocols that can transport packets of data from one device to another and check for errors along the way.
* TLS: A secure protocol for sending encrypted data so that attackers can't view private information.
* HTTP & DNS: The protocols powering the World Wide Web, what the browser uses every time you load a webpage.

## Network
A computer network is any group of interconnected devices capable of sending or receiving data.
* Local Area Network (LAN): Network covers limited area like house or school.
* Wide Area Network (WAN): Extend over a large geographic area and is composed of many LAN's.
* Data Center Network (DCN): used in data centers where data must be exchanged with very little delay.







