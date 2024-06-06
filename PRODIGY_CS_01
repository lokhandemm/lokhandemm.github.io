def caesar_cipher_encrypt(text, shift):
    encrypted_text = ""
    for char in text:
        if char.isalpha():
            shift_base = 65 if char.isupper() else 97
            encrypted_text += chr((ord(char) - shift_base + shift) % 26 + shift_base)
        else:
            encrypted_text += char
    return encrypted_text

def caesar_cipher_decrypt(text, shift):
    decrypted_text = ""
    for char in text:
        if char.isalpha():
            shift_base = 65 if char.isupper() else 97
            decrypted_text += chr((ord(char) - shift_base - shift) % 26 + shift_base)
        else:
            decrypted_text += char
    return decrypted_text

def main():
    choice = input("Do you want to (e)ncrypt or (d)ecrypt a message? ")
    if choice.lower() not in ['e', 'd']:
        print("Invalid choice! Please select 'e' to encrypt or 'd' to decrypt.")
        return
    
    message = input("Enter your message: ")
    shift = int(input("Enter the shift value: "))
    
    if choice.lower() == 'e':
        encrypted_message = caesar_cipher_encrypt(message, shift)
        print(f"Encrypted message: {encrypted_message}")
    elif choice.lower() == 'd':
        decrypted_message = caesar_cipher_decrypt(message, shift)
        print(f"Decrypted message: {decrypted_message}")

if __name__ == "__main__":
    main()
