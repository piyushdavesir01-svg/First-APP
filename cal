import streamlit as st

st.set_page_config(page_title="Simple Calculator")

st.title("🧮 Simple Calculator")

# Inputs
num1 = st.number_input("Enter first number:", value=0.0)
num2 = st.number_input("Enter second number:", value=0.0)

# Operation selector
operation = st.selectbox("Choose Operation", ["+", "-", "*", "/"])

# Calculate button
if st.button("Calculate"):
    try:
        if operation == "+":
            result = num1 + num2
        elif operation == "-":
            result = num1 - num2
        elif operation == "*":
            result = num1 * num2
        elif operation == "/":
            if num2 == 0:
                st.error("Cannot divide by zero")
                raise ZeroDivisionError
            result = num1 / num2

        st.success(f"Result: {result}")

    except:
        st.error("Error occurred!")
