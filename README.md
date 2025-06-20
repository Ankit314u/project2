import random
adjectives = ["Certified", "Global", "Senior", "Dynamic", "Virtual", "Professional", "Elite", "Quantum"]
roles = ["Meme", "Unicorn", "Cloud", "AI", "Crypto", "Banana", "Mood", "Space"]
suffixes = ["Strategist", "Engineer", "Manager", "Guru", "Consultant", "Wizard", "Officer", "Architect"]

def generate_fake_title():
    adj = random.choice(adjectives)
    role = random.choice(roles)
    suffix = random.choice(suffixes)
    return f"{adj} {role} {suffix}"
while True:
    fake_title = generate_fake_title()
    print("\nYour Fake Job Title is: 🌟", fake_title)

    # Step 5 (Optional): Ask for another
    again = input("\nWant another one? (yes/no): ").lower()
    if again != "yes":
        print("Okay! Hope you enjoyed your new career 😄")
        break
