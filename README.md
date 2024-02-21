![image](https://github.com/cwinfieldp/PythonPasswordGenerator/assets/149834667/71eb0831-5e46-4de0-bd67-8b7040787e93)

This Python project is a simple password generator that allows customization of the password composition by including or excluding uppercase letters, lowercase letters, digits, and special characters. The generated passwords are printed to the console.
Here's a breakdown of the code:

Character Sets:

![image](https://github.com/cwinfieldp/PythonPasswordGenerator/assets/149834667/ed59404c-bb9c-4a9a-93ae-88b8f715a725)

capital_let: Uppercase letters, small_let: Lowercase letters ,numbers: Digits, special_char: Special characters

Boolean Flags:
upper, lower, digits, and odd are boolean variables that determine whether to include each respective character set in the password.

![image](https://github.com/cwinfieldp/PythonPasswordGenerator/assets/149834667/60da0bde-351a-43d7-85ea-816dca00601b)

Combining Character Sets:
The finalpass variable is used to combine the selected character sets based on the boolean flags.

![image](https://github.com/cwinfieldp/PythonPasswordGenerator/assets/149834667/640a401a-7c0d-4563-b2a7-43564e3a579a)

Password Generation:

![image](https://github.com/cwinfieldp/PythonPasswordGenerator/assets/149834667/64860f06-0a43-489a-be88-0b2d38e466fc)

The code uses a loop (for x in range(howmuch)) to generate multiple passwords (howmuch times).
For each password, it uses random.sample(finalpass, length) to randomly select characters from the combined character sets, creating a password of the specified length.
The generated password is then printed to the console.
Customization:
You can customize the character sets and adjust the boolean flags to control the composition of the passwords.
The length variable sets the length of each generated password.
The howmuch variable determines how many passwords are generated.
Note: The use of random.sample ensures that the characters in each password are unique, but the overall order of characters may vary. If you want to allow repeated characters, you can use random.choices instead of random.sample. Additionally, consider using the secrets module for cryptographic applications.
