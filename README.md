def check_even_odd(num):
    if num % 2 == 0:
        return "Even"
    else:
        return "Odd"

def main():
    values = []
    n = int(input("Enter the number of values: "))
    for i in range(n):
        value = int(input("Enter a number: "))
        values.append(value)

    results = [check_even_odd(num) for num in values]

    print("Results:")
    for i in range(n):
        print(f"{values[i]} is {results[i]}")

if __name__ == "__main__":
    main()
