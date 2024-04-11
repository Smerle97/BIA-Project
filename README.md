Installed Packages 
  - Flask              3.0.3
  - openai             0.28.0
  - openpyxl           3.1.2
  - pandas             2.2.1
  - pip                23.2.1

This program is currently running flask as the main start to the chatbot
(if __name__ == '__main__':
    app.run(debug=True))

If we are just using the chatbot in python, you can use this code 

print("Welcome to the Financial Advisor Chatbot. Type 'exit' to end the conversation.")

while True:
    user_input = input("You: ")
    if user_input.lower() == 'exit':
        print("Exiting...")
        break
    response = CustomChatGPT(user_input)
    print("Assistant:", response)
