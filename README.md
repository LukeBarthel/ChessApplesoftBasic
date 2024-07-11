# ChessApplesoftBasic

This is a very simple Chess game written in Applesoft Basic. You can try it yourself on "https://www.calormen.com/jsbasic/", or on any other emulator by uploading the "Chess.txt".
![WhatsApp Bild 2024-07-11 um 12 42 06_f4487f04](https://github.com/LukeBarthel/ChessApplesoftBasic/assets/175216318/2ee47383-00ae-42d2-8996-efc8029cc7bb)

## 1. Variable Initilization

- hgr: Initializes high-resolution graphics mode.
- bp(15, 2): Array for black piece positions.
- wp(15, 2): Array for white piece positions.
- f: Frame buffer toggle.
- n: Is used to tell wich line of pieces are being created.
- sc: Scale factor for graphics.
- poke and call commands: Hardware and display initialization.
- d: Delay counter.
- gosub: Calls subroutines to define piece outlines.
- cb(63, 1): Array for the state of the chessboard.

## 2. Game Loop

First the Chess board is drawn, then the curser. Afterwards it loops over the key listener until the programm is terminated.

## 3. Draw setup

Here the Chess board is plotted and then the Pieces on top.

## 4. Player Input

Assigns the current key ID to variable k and then checks k for arrow keys and the space bar to perform the corresponding actions.
The Arrow keys move the curser and space grabs and places pieces.

## 5. Calculate Move

Is not jet finished

## 6. draw Curser

Clears the old Curser and draws new one.

## 7. Delay

Since Applesoft Basic doesn't support multiple threads or have an integrated timer, the most common way to create a delay is to loop over nothing, using a variable that represents the duration of the wait. This method is inaccurate, as the desired value has to be estimated through trial and error, and the duration won't be consistent because it is based on computing steps rather than actual time.

## 8. Define (...), Draw (...)

Every chesspiece's outline is defined and gets a function to draw it at a given position on the board.

## 9. Setup Board

Sets the predefined Pieces on their respective squares.

## 10. Check for picked up piece

Checks what needs to happen, when the space bar is pressed and executes it.

## 11. Draw square

Draws an Empty Square at a given Position.

## 12. Paste Piece

Pastes a copied piece at a given position.
