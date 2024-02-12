## Password Generator

### Introduction
This is a simple password generator program implemented in C. It allows users to generate passwords of varying strengths and lengths based on their preferences.

### Features
- Four levels of password strength: Weak, Moderate, Strong, and Very Strong.
- Customizable password length within the range of 6 to 20 characters.
- Random generation of passwords based on user-selected strength and length.
- Detection of ambiguous characters in generated passwords.
- Option to regenerate passwords or exit the program.

### Usage
1. **Strength Selection**: Users are prompted to select the desired strength level for the password generation (1-4).
2. **Length Selection**: Users choose the desired length of the password within the range of 6 to 20 characters.
3. **Password Generation**: The program generates a password based on the selected strength and length.
4. **Ambiguous Character Detection**: If the generated password contains ambiguous characters (like 'l', '1', 'I', 'o', '0', 'O'), it is indicated to the user.
5. **Try Again Option**: Users can choose to generate another password or exit the program.
6. **End of Program**: Upon choosing to exit, a thank you message is displayed, and the program terminates.

### Dependencies
- Standard C libraries: `stdio.h`, `stdlib.h`, `time.h`, `string.h`, `stdbool.h`, `math.h`

### Notes
- The program utilizes the `rand()` function for random number generation. For better randomness, consider using a more sophisticated random number generator.
- Ambiguous characters detection is based on a predefined set of characters. Modify the `ambiguous` array in the `has_ambiguous_characters` function to adjust the set of ambiguous characters according to your needs
