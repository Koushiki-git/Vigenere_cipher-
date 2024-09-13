Here's a short summary of the code:

1. File Reading (`textstrip`): Reads a file and returns a string containing only lowercase letters, filtering out all non-letter characters.
   
2. Letter Count (`count_distribution`): Counts the frequency of each lowercase letter in a string and stores it in a dictionary.

3. Substitution Cipher:
   - Encryption: Creates a random mapping of lowercase letters to uppercase and non-letter characters. The `substitution_encrypt` function uses this mapping to encrypt the text.
   - Decryption: The `substitution_decrypt` function reverses the encrypted text back to its original form using the reverse mapping.

4. Vigenere Cipher:
   - Encryption: Uses a keyword to shift each letter of the plaintext to an uppercase letter based on a repeating key pattern.
   - Decryption: Reverses the Vigenere encryption using the same key.

5. Cryptanalysis:
   - Vigenere Key Length Guessing: Uses letter collision analysis (`rotate_compare`) to predict the length of the Vigenere cipher key.
   - Key Guessing: Analyzes letter frequencies to guess the encryption key, assuming common English letter distributions.
   - Full Decryption: After determining the key, it decrypts the Vigenere cipher text and returns the guessed key and plaintext.
