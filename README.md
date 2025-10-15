1. Why is the Caesar cipher insecure?
Because it only has 26 possible shifts, so anyone can try all of them quickly. The letter patterns stay the same, so common letters and words are easy to spot. It gives no real protection.


2. First, the given text is written in Base64, which is not encryption but just an encoding.
So, the first thing to do is decode it from Base64 to get the real encrypted bytes.
Then, you use the passphrase found in Step 2 — which is “secure” — to decrypt it using XOR.
The XOR process takes each byte of the encrypted message and XORs it with the corresponding byte from the key (“secure”), repeating the key until the message is fully decrypted.
After this operation, the hidden message appears: “This is the XOR challenge!”
