```
def reverse_hex_string(hex_string):
    # Convert the space-separated hex string to a list of hex values
    data = hex_string.split()
    
    # Reverse the list
    reversed_data = data[::-1]
    
    # Join the reversed list back into a space-separated string
    reversed_hex_string = ' '.join(reversed_data)
    
    return reversed_hex_string

# Example usage
input_hex_string = "e8 b9 7b e4 85 b5 a5 ab ea dc 77 f2 bc 33 d9 2c 35 ed 23 05 2d 6d 2a 6f 0a ef 75 68 a1 53 3d a7 65 34 91 a1"
reversed_hex_string = reverse_hex_string(input_hex_string)

# Print the reversed hex string
print("Reversed hex string:")
print(reversed_hex_string)
```
