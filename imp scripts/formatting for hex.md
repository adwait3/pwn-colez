```
input_string = "9E 61 BC 2C 72 2C 67 6F 6A 6A 6C 6C 6C 6D 6D 68 6F 6F 70 88 BE 72 74 74 75 76 77 77 77 72 77 79 7A 7A 7A"
input_string = input_string.replace(" ", "")  # Remove spaces
output_string = "\\x" + "\\x".join(input_string[i:i+2] for i in range(0, len(input_string), 2))
print(output_string)
```
