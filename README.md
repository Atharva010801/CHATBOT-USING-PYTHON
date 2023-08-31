# CHATBOT-USING-PYTHON
import random

def chatbot_response(user_input):
    responses = [
        "Hello!",
        "How can I help you?",
        "Tell me more.",
        "I'm listening.",
        "That's interesting.",
        "Sorry, I don't have the answer right now.",
        "Let's talk about something else.",
        "I'm not sure I understand.",
        "Could you rephrase that?",
        "What do you think about that?",
    ]
    
    return random.choice(responses)

def main():
    print("Chatbot: Hello! How can I assist you today?")
    
    while True:
        user_input = input("You: ")
        if user_input.lower() == "bye":
            print("Chatbot: Goodbye! Have a great day!")
            break
        else:
            response = chatbot_response(user_input)
            print(f"Chatbot: {response}")

if __name__ == "__main__":
    main()
