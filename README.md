# Diodes and Rectifiers Calculator

print("DIODES AND RECTIFIERS")

print("\n1. Half-Wave Rectifier")
print("2. Full-Wave Rectifier")

choice = int(input("Enter your choice (1 or 2): "))

Vm = float(input("Enter peak input voltage (V): "))

# Diode forward voltage
Vd = float(input("Enter diode forward voltage (V): "))

# Output voltage calculation
if choice == 1:
    rectifier = "Half-Wave Rectifier"
    Vdc = (Vm - Vd) / 3.14159
    efficiency = 40.6

elif choice == 2:
    rectifier = "Full-Wave Rectifier"
    Vdc = 2 * (Vm - Vd) / 3.14159
    efficiency = 81.2

else:
    print("Invalid choice!")
    exit()

print("\n--- RESULTS ---")
print("Rectifier Type =", rectifier)
print("Peak Input Voltage =", Vm, "V")
print("Diode Forward Voltage =", Vd, "V")
print("Average DC Output Voltage =", round(Vdc, 2), "V")
print("Maximum Rectification Efficiency =", efficiency, "%")# diodes-and-rectifiers