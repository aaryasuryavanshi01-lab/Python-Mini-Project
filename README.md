# Python-Mini-Project
Pollution Calculator.

print("                               POLLUTION CALCULATOR      ")

print("Please enter all your data in capital letters.")
fuel=["PETROL","DIESEL","CNG"]
fuel=input("Enter which fuel you are using for your vehicle: ")
Running=float(input("Enter weekly running of your vehicle in litres: "))
print("---------------------------------------------------------------------------")
if(fuel=="PETROL"):
    print("Petrol contains ethanol(E10-E20).")
    ethanol=Running*0.10
    print("Ethanol present in your petrol (approx):",ethanol,"litres")
    CO2=Running*2.68
    print("Your weekly CO2 Emmision:",CO2,"kg")
elif(fuel=="DIESEL"):
    print("Diesel contains biodiesel (B5-B20).")
    biodiesel=Running*0.05
    print("Biodiesel present in your diesel (approx):",biodiesel,"litres")
    CO2=Running*2.31
    print("Your weekly CO2 Emmision:",CO2,"kg")
elif(fuel=="CNG"):
    print("CNG contains methane.")
    methane=Running*0.90
    print("Methane present in your CNG (approx):",methane,"litres")
    CO2=Running*2.75
    print("Your weekly CO2 Emmision:",CO2,"kg")
else:
    print("Error! Enter proper fuel name.")
print("---------------------------------------------------------------------------")
if(Running<=5):
    print("Pollution Level: LOW")
elif(Running<=15):
    print("Pollution Level: MODERATE")
else:
    print("Pollution Level: HIGH")
print("---------------------------------------------------------------------------")
if(Running<=5):
    print("Suggesition:Good.Maintain your vehicle regularly. ")
elif(Running<=15):
    print("Suggestion:Reduce unnecessary trips.")
else:
    print("Suggestion:Consider carpooling or public transport")
