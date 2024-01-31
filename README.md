#Witout GUI CODE 1


import time

def welcome_message():
    print("Welcome to our EatEase Restaurant ma'am & sir!")
    first_name = input("May I know your first name, please? ")
    print(f"Thank you, {first_name}! What would you like to order?")

food_menu = {
    1: {"name": "Adobo", "price": 172.00},
    2: {"name": "Bulalo", "price": 181.00},
    3: {"name": "Kare-kare", "price": 499.99},
    4: {"name": "Lumpia Shanghai with sauce", "price": 500},
    5: {"name": "Sinigang Small", "price": 245.00},
    6: {"name": "Sinigang Medium", "price": 455.00},
    7: {"name": "Sinigang Large", "price": 755.00},
    8: {"name": "Spaghetti Single", "price": 70.00},
    9: {"name": "Spaghetti 3-5 persons", "price": 540.00},
    10: {"name": "Spaghetti 6-10 persons", "price": 750.00},
    11: {"name": "Spaghetti 11-15", "price": 850.00},
    12: {"name": "Tinola", "price": 112.38}
}

soft_drinks_menu = {
    1: {"name": "Coke", "price": 1.99},
    2: {"name": "7up", "price": 20.00},
    3: {"name": "Royal", "price": 2.99},
    4: {"name": "Sprite", "price": 1.99},
}

def display_menu(menu, menu_name):
    print(f"\n{menu_name} Menu:")
    for number, item in menu.items():
        print(f"{number}: {item['name']} - ₱{item['price']:.2f}")

def restaurant_foods():
    display_menu(food_menu, "EatEase Food")
    choices = list(food_menu.keys())
    while True:
        request = input("\nPlease enter the number of your food choice: ")
        if request.isdigit() and int(request) in choices:
            print(food_menu[int(request)]['name'], "is available")
            print("Chief is cooking your order...")
            time.sleep(10) 
            print("Here's your Order! Enjoy your meal!")
            break
        else:
            print("Ready in 30 mins...")
            time.sleep(1)
            print("Sorry not available. Please choose from the food menu by entering the corresponding number.")
            display_menu(food_menu, "EatEase Food")
        
def soft_drinks():
    display_menu(soft_drinks_menu, "EatEase Soft Drinks")
    choices = list(soft_drinks_menu.keys())
    while True:
        request = input("\nPlease enter the number of your drink choice: ")
        if request.isdigit() and int(request) in choices:
            print(soft_drinks_menu[int(request)]['name'], "is available")
            print("Getting your order drink...")
            time.sleep(10)  
            print("Here's your Order! Enjoy your drink!")
            break
        else:
            print("Wait a minute...")
            time.sleep(1)
            print("Sorry not available. Please choose from the soft drinks menu by entering the corresponding number.")
            display_menu(soft_drinks_menu, "Soft Drinks")

welcome_message()
restaurant_foods()
soft_drinks()




#With GUI CODE 2



import time

def welcome_message():
    print("Welcome to our EatEase Restaurant ma'am & sir!")
    first_name = input("May I know your first name, please? ")
    print(f"Thank you, {first_name}! What would you like to order?")

food_menu = {
    1: {"name": "Adobo", "price": 172.00},
    2: {"name": "Bulalo", "price": 181.00},
    3: {"name": "Kare-kare", "price": 499.99},
    4: {"name": "Lumpia Shanghai with sauce", "price": 500},
    5: {"name": "Sinigang Small", "price": 245.00},
    6: {"name": "Sinigang Medium", "price": 455.00},
    7: {"name": "Sinigang Large", "price": 755.00},
    8: {"name": "Spaghetti Single", "price": 70.00},
    9: {"name": "Spaghetti 3-5 persons", "price": 540.00},
    10: {"name": "Spaghetti 6-10 persons", "price": 750.00},
    11: {"name": "Spaghetti 11-15", "price": 850.00},
    12: {"name": "Tinola", "price": 112.38}
}

soft_drinks_menu = {
    1: {"name": "Coke", "price": 1.99},
    2: {"name": "7up", "price": 20.00},
    3: {"name": "Royal", "price": 2.99},
    4: {"name": "Sprite", "price": 1.99},
}

def display_menu(menu, menu_name):
    print(f"\n{menu_name} Menu:")
    for number, item in menu.items():
        print(f"{number}: {item['name']} - ₱{item['price']:.2f}")

def restaurant_foods():
    display_menu(food_menu, "EatEase Food")
    choices = list(food_menu.keys())
    while True:
        request = input("\nPlease enter the number of your food choice: ")
        if request.isdigit() and int(request) in choices:
            print(food_menu[int(request)]['name'], "is available")
            print("Chief is cooking your order...")
            time.sleep(10) 
            print("Here's your Order! Enjoy your meal!")
            break
        else:
            print("Ready in 30 mins...")
            time.sleep(1)
            print("Sorry not available. Please choose from the food menu by entering the corresponding number.")
            display_menu(food_menu, "EatEase Food")
        
def soft_drinks():
    display_menu(soft_drinks_menu, "EatEase Soft Drinks")
    choices = list(soft_drinks_menu.keys())
    while True:
        request = input("\nPlease enter the number of your drink choice: ")
        if request.isdigit() and int(request) in choices:
            print(soft_drinks_menu[int(request)]['name'], "is available")
            print("Getting your order drink...")
            time.sleep(10)  
            print("Here's your Order! Enjoy your drink!")
            break
        else:
            print("Wait a minute...")
            time.sleep(1)
            print("Sorry not available. Please choose from the soft drinks menu by entering the corresponding number.")
            display_menu(soft_drinks_menu, "Soft Drinks")

welcome_message()
restaurant_foods()
soft_drinks()

