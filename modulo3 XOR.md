modulo 3 xor 
```
def modulo_3_xor_encryption(hex_string):
    # Convert the space-separated hex string to a list of integers
    data = [int(byte, 16) for byte in hex_string.split()]
    
    # Define the XOR keys for the encryption
    keys = [0x8d, 0x95, 0xe5]
    
    # Encrypt the data using modulo 3 XOR
    encrypted_data = []
    for i in range(len(data)):
        key = keys[i % 3]
        encrypted_byte = data[i] ^ key
        encrypted_data.append(encrypted_byte)
    
    return encrypted_data

# Example usage
input_hex_string = "1F 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F 10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 00"
encrypted_data = modulo_3_xor_encryption(input_hex_string)

# Print the encrypted data in hexadecimal format
print("Encrypted data:")
for byte in encrypted_data:
    print(f"{byte:02x}", end=" ")
print()

```

