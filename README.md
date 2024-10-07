# Round-1
Round 1 answer
# Function to fnd the second highest value in an array without sorting
def get_second_largest(numbers):
    if len(numbers) < 2:
        return None
    
    max_val = foat('-inf')
    second_max = foat('-inf')
    
    # Loop through each element in the array
    for value in numbers:
    
        if value > max_val:
            second_max = max_val
            max_val = value
    
        elif max_val > value > second_max:
            second_max = value
    
    
    if second_max == foat('-inf'):
        return None
    return second_max
example_array = [3, 12, 7, 4, 15, 9]
output = get_second_largest(example_array)
if output is not None:
    print("Second largest number is:", output)
else:
    print("No second largest number found");
