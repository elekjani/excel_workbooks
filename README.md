# Simple workbook to learn words or expression in multiple languages

This is a simple book to learn vocabulary for multiple different languages based on the card and boxes method. Each card can have multiple "side" that represents the different languages and the cards are in different boxes according how well one knows them. The first box (Box1) contains all the cards that one doesn't know and the last box (Box10) is for the words one knows the best. This is achieved by moving a card up by one through the boxes if we know the given word in all languages and moving down if we don't konw. Unfortunalety the latest version of this workbook cannot check whether we really know the word, but it's up to the user to enter in a cell the result (do not cheat :) ).

The book contains four sheets
1. Words
** List of words in different languages and a timestamp representing the last time the word was tested. The first column is an index that must be unique and continuous from 1 to the number of words (no check is implemented for this, it's up to the user filling up this sheet to meet this constraint).
2. Boxes
** _Do not edit this sheet_. Each column represents a box and the words are referred in the boxes by their indecies on the "Words" sheet. The top row is for a per box tally showing the number of words per box.
3. Probablities
** _Do not edit the fist and last columns_. To select a word for test, first a box is selected with the probabilities listed on this sheet. The default implementation defines these probabilities by the index of the boxes. The relative probability of the *n*th box is *1/n*. Arbitrary probablities can be defined in the *Probability* column, but the sum of those must be one. 
4. Question
** Main sheet to be used to test our knowledge. Four type of input can be given and these can be changed in the yellow box. On default the characters *1* and *2* represent the *I know this word* and *I don't know this word* (resp.) answers. One can reveal the answer without changing the position of the given word in the boxes and the empty answer will make the next question appear.
 
