# Script météo interactif ☀️🌡️

Ce projet contient un script Python qui permet de :

- Saisir votre prénom
- Indiquer la ville où vous vous trouvez
- Entrer la température actuelle en degrés Celsius
- Afficher la température convertie en Fahrenheit
- Prédire la température de la nuit

## Prérequis

- Python 3 installé sur votre machine

## Utilisation

Pour lancer le script, ouvrez un terminal dans le dossier du projet et tapez :

```bash
python weather.py

exemple
What's your name? Mélanie
What city are you currently? Paris
What is the temperature in Paris? 20
Hi Mélanie, you are in Paris and it is currently 20ºC or 68ºF.
I predict that tonight, the temperature will reach 10ºC or 50ºF.
Have a good day!

Extrait
first_name = input("What's your name? ")
city = input("What city are you currently? ")
celsius_temperature  = input(f"What is the temperature in {city}? ")

fahrenheit_temperature = (float(celsius_temperature) * 9/5) + 32
fahrenheit_temperature = round(fahrenheit_temperature)

welcome_message = f"Hi {first_name.capitalize()}, you are in {city.capitalize()} and it is currently {celsius_temperature}ºC or {fahrenheit_temperature}ºF."
print(welcome_message)

tonight_celsius_temperature = float(celsius_temperature) - 10
tonight_celsius_temperature = round(tonight_celsius_temperature)
tonight_fahrenheit_temperature = (float(tonight_celsius_temperature) * 9/5) + 32
tonight_fahrenheit_temperature = round(tonight_fahrenheit_temperature)

prediction_message = f"I predict that tonight, the temperature will reach {tonight_celsius_temperature}ºC or {tonight_fahrenheit_temperature}ºF."
print(prediction_message)

print("Have a good day!")
