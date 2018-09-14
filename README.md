# LOB-ITCH-4.0
Limit Order Book for BIST 100

This is an ITCH implementation for BIST 100.
This implementation is adapted from an already existing itch-order book for a higher version.
It uses a hashmap to access every single order when needed.
Every other operation is done via vectors. For description and implementation see order_book.h.

Protocol specification: http://www.borsaistanbul.com/docs/default-source/nasdaq-dokuman/b%c4%b1stech-%c4%b1tch-protocol-specification.pdf?sfvrsn=4

Counting add,delete and execute orders as a packet, it can handle a packet in ~128 nanoseconds.
I/O needs ~ 40 nanoseconds.
Book handling operations cost ~ 20 nanoseconds.
If you have enough RAM, convert the hashmap to a vector, produce a unique number from order ID, order book ID and side. Use that unique number as the index. In this case performance is expected to double.
