# CS3700_Project1

I started off by creating a function for creating a TCP socket as well as connect it. From there, I initialized the different variables I would need, such as the "hello" message and the list of words to choose from. Then I sent the first message and then sent the code into a loop to keep guessing and eliminating words from the word list. Upon sending the "hello" message, I received the message back and stored the ID from it to use for future guesses. 

In order to guess, I used a random int generator to select which index to randomly pick a word out of the word list, and after each subsequent guess, I would eliminate words from the word list if the word in the word list had the same letter at the same position as the guessed word while also receiving a mark of '0' or '1'.

After receiving the flag from the correct guess, I used a print statement to print out the flag and then I would manually record it in secret_flags. Initially, I did not use an args parser to record commands in the command line, but rather hard coded values so that I could ensure my guessing algorithm was functional. After confirming, I implemented the args parser to take in the different fields in the command line and use them as the hostname, port, type of socket, and northeastern username.

To test and ensure that my code was working, I did not use args parse initially as stated before, and after args parse was implemented, I used print statements within the code that I later removed in order to ensure that certain parts of my code were being reached and were outputting the correct outputs. I verified the validity of the messages both sent and received by using variables that confirmed they were dictionaries with certain keys or values.
