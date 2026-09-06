appliances={}
for i in range(3):
  name=input("Enter appliance name :")
  power=float(input("Enter appliance power(watts) :"))
  hours_per_day=float(input("Enter hours used per day :"))
  days_per_week=int(input("Enter days used per week :"))
  appliances[name]={
    "power" : power,
    "hours_per_day" : hours_per_day,
    "days_per_week" : days_per_week
  }
  total_energy_consumption=0
  highest_energy_consumption=0
  highest_energy_appliance=""
  lowest_energy_consumption=1000000000000
  lowest_energy_appliance=""
  for appliance,details in appliances.items():
    power_nw=details["power"]/1000
    energy_consumption=power_nw*details["hours_per_day"]*details["days_per_week"]

    details["energy_consumption"]=energy_consumption
    total_energy_consumption+=energy_consumption
    if energy_consumption>highest_energy_consumption:
       highest_energy_consumption=energy_consumption
       highest_energy_appliance= appliance
    elif energy_consumption<lowest_energy_consumption:
       lowest_energy_consumption=energy_consumption
       lowest_energy_appliance= appliance
print(appliances)
print("Total Household Consumption:",total_energy_consumption,"KWH Per week")
print("Highest energy consuming appliance:",highest_energy_appliance )
print("Energy consumption: ",highest_energy_consumption,"KWH Per week")
print("Lowest energy consuming appliance:",lowest_energy_appliance )
print("Energy consumption: ",lowest_energy_consumption,"KWH Per week")
def analysis(b,p):
    print("Your",b,"is your highest energy consuming appliance with",p ,"KWH per week.Consider reducing its usage to lower household consumption")
    if p>5:
      print("This is also higher than the maximum usage of any home appliances therefore the reduction is a must")
    elif p>=1:
      print("However this is a moderate usage of home appliance so a reduction is not necessary")
    else:
      print("However this is a very minimal usage of a home appliance so pose no threat")
recommendations= analysis(highest_energy_appliance,highest_energy_consumption)
print(recommendations)
