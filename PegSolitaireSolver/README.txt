Peg Solitare

   peg-client.c0   - Client side implementation for stacks and hash tables
   peg1.c0         - Peg solitaire

Data:
   german.txt      - A trivial-to-solve board
   english.txt     - A board that you may be able to solve with peg2.c0 if 
                     you pick a very good move selection strategy (see 
                     Appendix A)
   french1.txt     - A difficult-to-solve board (but one with a solution)
   french2.txt     - A difficult-to-solve board (but one with a solution)
   french3.txt     - A difficult-to-solve-board (but one with a solution)

==========================================================

Compiling and running on the german board with -d:
   % cc0 -d -w -o peg1 peg-client.c0 lib/*.c0 peg1.c0 peg-main.c0
   % ./peg1 german.txt

   % cc0 -d -w -o peg2 peg-client.c0 lib/*.c0 peg2.c0 peg-main.c0
   % ./peg2 german.txt

   % cc0 -d -w -o peg3 peg-client.c0 lib/*.c0 peg3.c0 peg-main.c0
   % ./peg3 german.txt

Compiling and running on the english board. These direction give you
the fastest possible code, but use at your own risk!
   % cc0 -w -o peg2 -r unsafe -c-O2 peg-client.c0 lib/*.c0 peg2.c0 peg-main.c0
   % ./peg2 english.txt

   % cc0 -w -o peg3 -r unsafe -c-O2 peg-client.c0 lib/*.c0 peg3.c0 peg-main.c0
   % ./peg3 english.txt

==========================================================
