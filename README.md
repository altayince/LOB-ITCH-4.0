# LOB-ITCH-4.0
Limit Order Book for BIST 100

This is an ITCH implementation for BIST 100.
This implementation is adapted from an already existing itch-order book for a higher version.
It uses a hashmap to access every single order when needed.
Every other operation is done via vectors. For description and implementation see order_book.h.

Protocol specification: http://www.borsaistanbul.com/docs/default-source/nasdaq-dokuman/b%c4%b1stech-%c4%b1tch-protocol-specification.pdf?sfvrsn=4
