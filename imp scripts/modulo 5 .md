```
def xor_with_key(data, key):
    key_length = len(key)
    return [data[i] ^ key[i % key_length] for i in range(len(data))]

def hex_string_to_bytes(hex_string):
    return [int(byte, 16) for byte in hex_string.split()]

def bytes_to_hex_string(byte_list):
    return ' '.join(f'{byte:02x}' for byte in byte_list)

# Input hex string and key
input_hex_string = "a1 91 34 65 a7 3d 53 a1 68 75 ef 0a 6f 2a 6d 2d 05 23 ed 35 2c d9 33 bc f2 77 dc ea ab a5 b5 85 e4 7b b9 e8"
key_hex_string = "ed 1b 2f b3 ae"

# Convert hex strings to byte lists
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
