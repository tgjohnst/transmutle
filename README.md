# **Transmutle: The Word Alchemy Puzzle**

Hosted at: https://tgjohnst.github.io/transmutle

## **Concept**

Transmutle is a word puzzle game where players don't guess the target word directly. Instead, they "transmute" an initial five-letter starting word into a hidden five-letter target word through a series of allowed letter-transformation "recipes" or "runes." Each guess is an attempt to apply a valid transformation.

## **Gameplay**

1. **Starting & Target Words:** The game provides a starting five-letter word (e.g., "WATER") and a hidden target five-letter word (e.g., "FLAME").  
2. **Essence:** Players start with a limited amount of "Essence" (default: 20). Each rune activation costs a certain amount of essence.  
3. **Transformation Runes:** Players use a grimoire of "Transformation Runes" to alter the current word. Each rune has a specific effect and essence cost.  
4. **Applying Runes:**  
   * Click on a rune symbol to select it.  
   * The rune's details (name, cost, description) will appear below the rune symbols.  
   * Input fields for the rune's parameters (e.g., position, new letter) will appear below the rune details.  
   * For position inputs (1-5), you can either type the number or click directly on the desired letter tile in the "Current Word" display.  
   * Once parameters are set, click the "Transmute with \[Rune Name\]" button.  
5. **Feedback:**  
   * The game shows the resulting word after the transformation.  
   * Standard Wordle-like color clues (Green, Yellow, Grey) are then given, comparing the newly transmuted word to the hidden target word:  
     * **Green:** Correct letter in the correct position.  
     * **Yellow:** Correct letter in the wrong position.  
     * **Grey:** Letter not in the target word.  
   * The "Essence Remaining" is updated.  
   * The transmutation is recorded in the "Transmutation History."  
6. **Objective:** Transmute the starting word into the hidden target word using the allowed transformation runes before running out of "Essence."

## **Runes & Costs**

The following runes are available:

1. **Single Letter Swap (✎)**  
   * **Cost:** 3 Essence  
   * **Description:** Change one letter (position 1-5) to any other letter.  
   * **Inputs:** Position (1-5), New Letter (A-Z).  
2. **Positional Transposition (↔)**  
   * **Cost:** 1 Essence  
   * **Description:** Swap letter at position (1-5). Position 1-4 swaps with the letter to its right; Position 5 swaps with Position 1 (wraparound).  
   * **Inputs:** Position to swap (1-5).  
3. **Vowel/Consonant Cycle (↻)**  
   * **Cost:** 2 Essence  
   * **Description:** Cycle a letter at a position (1-5) to the next vowel (A→E→I→O→U→A) or consonant (B→C→D...).  
   * **Inputs:** Position of letter (1-5).  
4. **Elemental Affinity Shift (✦)**  
   * **Cost:** 4 Essence  
   * **Description:** Shift a letter at a position (1-5) to a random letter present in the hidden target word.  
   * **Inputs:** Position of letter (1-5).  
5. **Clone Letter (⊕)**  
   * **Cost:** 2 Essence  
   * **Description:** Clone letter from a source position (1-5) to a target position (1-5), overwriting the letter at the target position.  
   * **Inputs:** Source Position (1-5), Target Position (1-5).

## **How to Play Locally**

1. Save the HTML code as an .html file (e.g., transmutle.html).  
2. Open this file in a modern web browser.

## **Game Controls**

* **Rune Buttons:** Click to select a rune. Hover to see details.  
* **Letter Tiles (Current Word):** Clickable to select a position when a rune requiring position input is active.  
* **Input Fields:** Type in parameters for the selected rune.  
* **Transmute Button:** Applies the selected rune with the given parameters.  
* **New Game Button:** Starts a new game with new random start and target words, and resets essence.  
* **Play Again Button (in Game Over modal):** Restarts the game with new random words.

## **Technologies Used**

* HTML  
* CSS (Tailwind CSS)  
* JavaScript (Vanilla)

## **Future Enhancements (Ideas)**

* More diverse word lists or themed word lists.  
* Additional, more complex runes with unique effects.  
* Limited uses for certain powerful runes.  
* A "Hint" system that costs essence.  
* Difficulty levels (e.g., less starting essence, different word list complexity).  
* Score tracking or statistics.  
* Sound effects or improved visual feedback for transmutations.  
* Saving game progress (e.g., using localStorage or a backend).
