case study 2 of python 
NAME -  ARYAN SINGH 
ECE - A  
U.ID - 202501100700047 
KIET Group of institutions 




# Temperature Monitoring System 
import random 
import time 
# Accept minimum and maximum temperature limits 
min_temp = float(input("Enter minimum temperature limit: ")) 
max_temp = float(input("Enter maximum temperature limit: ")) 
# Number of readings to generate 
n = int(input("Enter number of temperature readings: ")) 
print("\nTemperature Monitoring Started...\n") 
for i in range(n): 
# Generate random temperature value 
current_temp = random.uniform(min_temp - 10, max_temp + 10) 
print("Temperature Reading", i + 1, ":", round(current_temp, 2), 
"°C") 
# Compare temperature with limits 
if current_temp < min_temp: 
print("Status: LOW Temperature Alert!\n") 
elif current_temp > max_temp: 
print("Status: HIGH Temperature Alert!\n") 
else: 
print("Status: Temperature is NORMAL\n") 
# Wait for 2 seconds 
time.sleep(2) 
print("Monitoring Finished.")
