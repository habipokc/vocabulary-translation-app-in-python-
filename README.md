# vocabulary-translation-app-in-python-
A vocabulary learning exercise application written using pandas and tkinter
First, the necessary libraries are imported: pandas, which is a powerful data analysis tool, and tkinter, which is a GUI toolkit for Python.

The BACKGROUND_COLOR variable is defined, which will be used later to set the background color of the GUI.

The current_card and to_learn variables are defined as empty dictionaries. The to_learn dictionary will eventually contain all of the words that the user needs to learn.

The try-except block is used to check if there is a CSV file named "words_to_learn.csv" in the data folder. If it exists, the data is read from the file and loaded into the to_learn dictionary. If it doesn't exist, the original data is read from the "french_words.csv" file and loaded into the to_learn dictionary.

The next_card function is defined. This function selects a random card from the to_learn dictionary, updates the GUI to display the French word on the front of the card, and sets a timer to automatically flip the card over after 3 seconds.

The flip_card function is defined. This function updates the GUI to display the English word on the back of the card.

The is_known function is defined. This function removes the current card from the to_learn dictionary, updates the CSV file, and calls the next_card function to display a new card.

The GUI is initialized using the Tkinter library. The title of the GUI is set to "Flashy", and the padding and background color are set.

A timer is set to automatically flip the card over after 3 seconds.

The canvas is initialized, which is where the flashcards will be displayed. Two images are loaded, one for the front of the card and one for the back of the card. The background image of the canvas is set to the front of the card image. Two text objects are created for the title and word on the card. The font, size, and color of the text are set.

The canvas is configured to have no border and is placed in the first row of the GUI.

Two buttons are created and placed in the second row of the GUI. One button displays a cross image and the other displays a check image. These buttons are used to indicate whether or not the user knows the word on the card.

The next_card function is called to display the first flashcard.

Finally, the mainloop function is called to start the GUI and wait for user input.


extra: when you want to customize, you can easily load words with help from googlesheet.
