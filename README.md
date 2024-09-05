# Hangman_Games
In the game of Hangman, the server chooses a random secret word from a list. It then shows the player a row of underscores, each representing a letter in the word. The player must guess letters, one by one.

If the player guesses a correct letter, it will be revealed in all the correct positions in the word, along with any letters that have already been guessed correctly.
If the player guesses a wrong letter, it's counted as an incorrect guess.
The player wins if they guess all the letters in the word. They lose if they make six incorrect guesses.
You need to write a "guess" function that takes the current state of the word (with some letters and underscores) and returns a guessed letter. This will be used to play 1,000 games of Hangman using the provided API. You can practice before submitting your results.

You are allowed to use a provided training set of about 250,000 dictionary words to improve your algorithm. However, the final test will be on a completely different set of 250,000 words that don't appear in the training set.

The basic algorithm works by matching the current word (with blanks) to possible words in the dictionary, counting how often letters appear, and guessing the most common letter that hasn’t been guessed yet. If no words match, it guesses based on overall letter frequency in the dictionary.

Your goal is to create an algorithm that does better than this basic one, which wins around 18% of the time.







