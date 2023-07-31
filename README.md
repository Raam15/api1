def get_weather_data(location, date):

def get_wind_speed_data(location, date):

def get_pressure_data(location, date):
def main():
    while True:
        print("1. Get weather\n2. Get Wind Speed\n3. Get Pressure\n0. Exit")
        choice = input("Enter your choice: ")

        if choice == '1':
            date = input("Enter the date (YYYY-MM-DD): ")
            temperature = get_weather_data("London", date)
            print(f"The temperature on {date} in London is {temperature}°C.")
        elif choice == '2':
            date = input("Enter the date (YYYY-MM-DD): ")
            wind_speed = get_wind_speed_data("London", date)
            print(f"The wind speed on {date} in London is {wind_speed} mph.")
        elif choice == '3':
            date = input("Enter the date (YYYY-MM-DD): ")
            pressure = get_pressure_data("London", date)
            print(f"The pressure on {date} in London is {pressure} hPa.")
        elif choice == '0':
            print("Terminating the program.")
            break
        else:
            print("Invalid choice. Please try again.")

if _name_ == "_main_":
    main()
