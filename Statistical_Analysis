# Set directory

# Load Data
data <- read.csv("shedder_data.csv")

# Check it Loaded
head(data)

## 01. Fisher's Exact Test
# Create a contingency table for Lotion and Shedder
lotion_table <- table(data$Lotion, data$Shedder)

#Check
lotion_table

# Run Test
fisher.test(lotion_table)

# Repeat for Race and Shedder
race_table <- table(data$Race, data$Shedder)
race_table
fisher.test(race_table)

## 02. Kruskal-Wallis Test
kruskal.test(DNA_Quantity ~ Lotion, data = data) # Test lotion effects
kruskal.test(DNA_Quantity ~ Race, data = data) #Test race effects
