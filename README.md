# Calculating age in years and months from a timedelta
# Todays date according to your computer
today  = dt.date.today()
# Any birthdate expressed as year, month, day
birthdate = dt.date(1993, 3, 3)
# Duration between the dates as a timedelta
delta_age = (today - birthdate)
# Duration between the dates as a number of days
days_old = delta_age.days
# Floor divide days by 365 to get the number of years
years = days_old // 365
# Days Left over is remainder of days_old divided by 365
# Floor divide that remainder by 30 for approximate months
months = (days_old % 365) // 30
# Print in a format to your liking
print(f"You are {years} years and {months} months old.")
