# TSN-timestables
# Creating times table checker week 10
def valid_integer():
    not_valid = True
    while not_valid:
        try:
            number = int(input())
            not_valid = False
        except ValueError:
            print("You must enter a number")
    return number
print("Welcome to the times table generator.") 
print("Enter a times table that you would like to display:")
times_table = valid_integer()
print("Enter the maximum value for your times table:")
max_value = valid_integer()
max_value = max_value + 1
answer = 0
print(f"Here is the {times_table} times table")
for x in range(1, max_value):
    answer = x * times_table
    print(f"{x} times {times_table} is {answer}")
