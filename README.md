# Activity
Github 1st Activity

import datetime

def calculate_age():
    print("--- Welcome to the Age Calculator! ---")

    current_year = datetime.datetime.now().year
    
    try:

        birth_year = int(input("Enter your birth year (e.g., 1995): "))
        

        if birth_year > current_year:
            print("Are you from the future? Please enter a valid birth year.")
            return
        elif birth_year < 1900:
            print("Wow, you might be the oldest person alive! Please enter a realistic year.")
            return
            

        age = current_year - birth_year
        print(f"\nYou are approximately {age} years old this year! 🎉")
        
    except ValueError:
        print("Invalid input! Please enter a 4-digit number for the year.")

if __name__ == "__main__":
    calculate_age()

