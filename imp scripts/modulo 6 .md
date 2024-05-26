```
def xor_with_key(data, key):
    key_length = len(key)
    return bytes(data[i] ^ key[i % key_length] for i in range(len(data)))

def hex_string_to_bytes(hex_string):
    return bytes.fromhex(hex_string)

def bytes_to_hex_string(byte_list):
    return ' '.join(f'{byte:02x}' for byte in byte_list)

# Input hex string and key
input_hex_string = "14 92 ea 8e 11 21 10 96 e1 83 1a 2b 18 81 f9 98 06 36 06 83 fb 9a 04 35 04 82 fd 9d 00 31 00 86 f1 90 0f 3f"
key_hex_string = "77 f1 89 e8 76 46"

# Convert hex strings to bytes
input_bytes = hex_string_to_bytes(input_hex_string)
key_bytes = hex_string_to_bytes(key_hex_string)

# Perform XOR encryption
encrypted_bytes = xor_with_key(input_bytes, key_bytes)

# Convert the encrypted bytes back to a hex string
encrypted_hex_string = bytes_to_hex_string(encrypted_bytes)

# Print the encrypted hex string
print("Encrypted hex string:")
print(encrypted_hex_string)
```
