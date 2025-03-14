# Enigma_Bombe
Implementation of a simulator for the M1 variant of the Enigma machine and a simplified version of the Turing Bombe (A more complex version will hopefully be complete soon). The following sections detail the implementations.

To verify encryption and decryption, two external simulators can be used: a) Cryptii Enigma Machine Simulator b) CacheSleuth Enigma Simulator

Please note that in these simulators, the "Rotor 1" is the leftmost rotor.

ENIGMA:

For the Enigma simulation, we created four classes: a) Rotor b) Reflector c) PlugBoard d) EnigmaMachine

Rotor configurations:

Rotor 1: ABCDEFGHIJKLMNOPQRSTUVWXYZ, Turnover: Q

Configuration: EKMFLGDQVZNTOWYHXUSPAIBRCJ
Rotor 2: ABCDEFGHIJKLMNOPQRSTUVWXYZ, Turnover: E

Configuration: AJDKSIRUXBLHWTMCQGZNPYFVOE
Rotor 3: ABCDEFGHIJKLMNOPQRSTUVWXYZ, Turnover: V

Configuration: BDFHJLCPRTXVZNYEIWGAKMUSQO
Rotor 4: ABCDEFGHIJKLMNOPQRSTUVWXYZ, Turnover: J

Configuration: ESOVPZJAYQUIRHXLNFTGKDCMWB
Rotor 5: ABCDEFGHIJKLMNOPQRSTUVWXYZ, Turnover: Z

Configuration: VZBRGITYUPSDNHLXAWMJQOFECK
Reflector "B" Configuration: ABCDEFGHIJKLMNOPQRSTUVWXYZ : YRUHQSLDPXNGOKMIEBFZCWVJAT

How to Run the Code:

Using the terminal, navigate to the folder where the code file is present.
Type python <file_name>.py and press enter to run the code.
Input Format:

Rotor choice and order: 3 space-separated integers (1-5).
Rotor settings: 3 space-separated alphabets.
Ring settings: 3 space-separated alphabets.
Plugboard connections: Space-separated alphabet pairs (e.g., ab fg ed tg). Type 'nop' if no plugboard is used.
Choose between encryption or decryption.
Enter the text for the chosen operation.
BOMBE:

Below is presented a simplified version of the Turing Bombe without loops and graphs. (A more complex version will hopefully be added soon)

How to Run the Code:

Using the terminal, navigate to the folder where the code file is present.
Type python <file_name>.py and press enter to run the code.
Input Format: a) Text to be fed: Enter the text for which the solution will be found. b) Hint: This is the guess for crib matching. c) Initial guess of rotors: 3 space-separated integers (1-5).

If no solutions are found for a given choice of rotors, additional guesses can be entered. Once solutions are found, no further input is required.

The final output will be all the solutions found for the inputted rotor settings
