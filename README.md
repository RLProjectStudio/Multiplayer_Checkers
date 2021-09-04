# Multiplayer_Checkers

## Introduction

A simple 2-player console Checkers game written in C++.

This game utilizes TCP/IP and is connected through an instance of a non-interactive server program.

## How to Run

Download both the `server.exe` and `client.exe` applications. Navigate to the directory where the application has been downloaded and run the `cmd` on Windows. 

Start the **Server** application and enter the number of a network port on which it will listen for TCP/IP connections as a command-line parameter.

![Screenshot 2021-09-05 044607](https://user-images.githubusercontent.com/89937219/132107898-940cf265-e428-4086-b08f-de4cdea22cbd.png)

After the server application has been started, start the **Client** application. 

Enter the player configurations as command-line parameters in the format of 

`client.exe hostname portnumber playername`

![Screenshot 2021-09-05 045104](https://user-images.githubusercontent.com/89937219/132107949-28a4c540-c340-4336-889f-f03785219051.png)

The game starts when 2 players have connected to the game.

![Screenshot 2021-09-05 050354](https://user-images.githubusercontent.com/89937219/132108009-94c02932-a42b-4df4-9bf6-6fa761fea1a7.png)

## How to Play

The standard rules of Checkers applies. Players are only allowed to move their respective pieces during their turn. Pieces are converted to King pieces upon reaching the last row across the board. Normal pieces are only allowed to forward while King pieces are allowed both forward and backward movement.

To move pieces, the player enters the commands in the format of
`move [from] [to]`

For example, the command `move D6 E5` moves the white piece from D6 to E5.

![Screenshot 2021-09-05 051333](https://user-images.githubusercontent.com/89937219/132108204-46bed698-5458-46a5-b399-a1f132ec97d3.png)

To skip a move, the player can enter the command `skip` to pass the turn to the opposing player.

## How to Terminate

The game is terminated when the game ends after the winner is announced. To terminate the game midgame, the player can enter the command `quit`.

## Credits

This game was completed solo as part of a school networking assignment and hence its source code cannot be published.
