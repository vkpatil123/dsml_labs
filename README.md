# dsml_labs
#asg 14
# Step 1: Import required libraries
import pandas as pd

df = pd.read_csv("/content/drive/MyDrive/Datasets/Covid Vaccine Statewise.csv")

print("Dataset Description:")
print(df.info())
print("\nFirst 5 rows of the dataset:")
print(df.head())

print("\nNumber of Males vaccinated:")
# Sum up the males vaccinated column
males_vaccinated = df['Male(Individuals Vaccinated)'].sum()
print(f"Total number of males vaccinated: {males_vaccinated}")

# Step 5: Number of Females Vaccinated
print("\nNumber of Females vaccinated:")
# Sum up the females vaccinated column
females_vaccinated = df['Female(Individuals Vaccinated)'].sum()
print(f"Total number of females vaccinated: {females_vaccinated}")
