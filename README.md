# fake_headline_generator
import random

subjects = [
    "Shah Rukh Khan",
    "Virat Kohli",
    "Nirmala Sitharaman",
    "A Mumbai cat",
    "A group of monkeys",
    "Prime Minister Modi",
    "An auto rickshaw driver from Delhi"
]

actions = [
    "launches",
    "cancels",
    "dances with",
    "eats",
    "declares war on",
    "orders",
    "celebrates"
]

places_or_things = [
    "at Red Fort",
    "in a Mumbai local train",
    "a plate of samosa",
    "inside Parliament",
    "at Ganga ghat",
    "during an IPL match",
    "at India Gate"
]

while True:
    subject = random.choice(subjects)
    action = random.choice(actions)
    place_or_thing = random.choice(places_or_things)

    headline = f"🚨 BREAKING NEWS: {subject} {action} {place_or_thing}"
    print("\n" + headline)

    user_input = input("\nAnother headline? (yes/no): ").strip().lower()
    if user_input not in ["yes", "y"]:
        break
