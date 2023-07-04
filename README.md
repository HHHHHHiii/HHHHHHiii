def solve_math_expression(expression):
    try:
        result = eval(expression)
        return result
    except Exception as e:
        return f"Error: {e}"

if __name__ == "__main__":
    print("Welcome to the Math Solver!")
    print("Enter a mathematical expression or type 'exit' to quit.")
    
    while True:
        user_input = input(">> ")
        if user_input.lower() == 'exit':
            print("Exiting the Math Solver.")
            break
        
        result = solve_math_expression(user_input)
        print("Result:", result)
