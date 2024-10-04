# 🚀 Flashy: A Flashcard Language Learning App

This is a simple flashcard application built using Python's `tkinter` for GUI and `pandas` for data manipulation. The purpose of this application is to help users learn French vocabulary through an interactive flashcard approach. 🇫🇷✨

## ✨ Features

- 📚 Flashcards display French words with English translations after a delay.
- ✅ User can mark words they know, which removes them from the vocabulary list to focus on unfamiliar words.
- 💾 Saves user progress between sessions so that previously learned words do not reappear.

## 🚀 How to Use

1. Run the Python script to launch the application.
2. 📝 The app will display a flashcard with a French word.
3. ⏱ After 3 seconds, the flashcard will automatically flip to show the English translation.
4. ✅ If you know the word, click the "check" button. The word will be removed from the vocabulary list.
5. ❌ If you do not know the word, click the "cross" button, and it will appear again in future sessions.
6. 🔄 Your progress will be saved automatically in `data/words_to_learn.csv`.

## 🛠 Installation

### Prerequisites
- 🐍 Python 3.x
- The following Python libraries:
  - `tkinter`
  - `pandas`
  - `random`

To install the necessary libraries, you can use:
```sh
pip install pandas
```

### Running the Application
1. 📂 Clone the repository to your local machine.
2. ✅ Ensure that the `data` folder contains the `french_words.csv` file with vocabulary words to start.
3. 🖼 Ensure the `images` folder contains the following images:
   - `card_front.png` (flashcard front image)
   - `card_back.png` (flashcard back image)
   - `wrong.png` (button image for unknown words)
   - `right.png` (button image for known words)
4. ▶️ Run the script:
   ```sh
   python flashy.py
   ```

## 📁 File Structure

- **data/french_words.csv**: 📋 Contains the list of French words with their English translations.
- **data/words_to_learn.csv**: ✏️ Updated by the application with words that are still to be learned.
- **images/**: 🖼 Contains all image files used in the application.

## 📝 Code Overview

- The application makes use of `tkinter` for creating the GUI, `pandas` for manipulating CSV data, and `random` for selecting words randomly.
- **next_card()**: 🃏 Displays a new French word.
- **flip_card()**: 🔄 Flips the card to reveal the English translation.
- **is_known()**: 🗑 Removes the current word from the learning list and updates the progress.

## 📸 Screenshot
![image](https://github.com/user-attachments/assets/f13ed08d-2c49-46cf-a5a1-2f6bf9ba38e8)


## 🤝 Contributing

Feel free to fork this repository, make improvements, and create pull requests. Your contributions are welcome! 🎉

## 📜 License

This project is licensed under the MIT License. 📄
