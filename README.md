# robo-speakers-for-windows
Robo speaker
import pyttsx3
print("Welcome to RoboSpeaker 1.1 Created by M TAQI")

# Initialize the pyttsx3 engine
engine = pyttsx3.init()
engine.setProperty('volume', 5.5)

while True:
    # Get user input
    text = input("Enter text to speak (press q to quit): ")

    # Check if the user wants to quit
    if text.lower() == "q":
        print ("thanks for using this robo speakers")
        break

    # Use the engine to speak the text
    engine.say(text)

    # Run the engine in the backgroundlayyah
    engine.runAndWait()
