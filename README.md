# Load necessary libraries 

library(ggplot2) library(dplyr) 

# Load the dataset (assuming the CSV file is named 

"credit_card_data.csv" and is in the working directory) credit_data <-

read.csv("creditcard_tb.csv", header = TRUE) 

# Display the structure of the dataset str(credit_data) 

# Summary statistics of the dataset summary(credit_data) 

# Check for missing values 

missing_values <- colSums(is.na(credit_data)) print(missing_values)# Check the class distribution of the target variable (assuming the target variable is 

named "Class") 

class_distribution <- table(credit_data$Class) print(class_distribution) 

# Visualize the class distribution using a bar plot 

barplot(class_distribution, main = "Class Distribution", xlab = "Class", ylab = 

"Frequency", col = c("green", "red"), legend = c("Non-Fraud", 

"Fraud")) 

# Plot some exploratory data analysis (EDA) plots (assuming V1-V28 are the 

features) 

# For example, histograms of some features for both classes 

ggplot(credit_data, aes(x = V1, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution of V1 

by Class") + xlab("V1") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal() 

ggplot(credit_data, aes(x = V2, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution 

of V2 by Class") + xlab("V2") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal()# Load necessary libraries 

library(ggplot2) library(dplyr) 

# Load the dataset (assuming the CSV file is named 

"credit_card_data.csv" and is in the working directory) credit_data <-

read.csv("creditcard_tb.csv", header = TRUE) 

# Display the structure of the dataset str(credit_data) 

# Summary statistics of the dataset summary(credit_data) 

# Check for missing values 

missing_values <- colSums(is.na(credit_data)) print(missing_values)# Check the class distribution of the target variable (assuming the target variable is 

named "Class") 

class_distribution <- table(credit_data$Class) print(class_distribution) 

# Visualize the class distribution using a bar plot 

barplot(class_distribution, main = "Class Distribution", xlab = "Class", ylab = 

"Frequency", col = c("green", "red"), legend = c("Non-Fraud", 

"Fraud")) 

# Plot some exploratory data analysis (EDA) plots (assuming V1-V28 are the 

features) 

# For example, histograms of some features for both classes 

ggplot(credit_data, aes(x = V1, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution of V1 

by Class") + xlab("V1") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal() 

ggplot(credit_data, aes(x = V2, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution 

of V2 by Class") + xlab("V2") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal()# Load necessary libraries 

library(ggplot2) library(dplyr) 

# Load the dataset (assuming the CSV file is named 

"credit_card_data.csv" and is in the working directory) credit_data <-

read.csv("creditcard_tb.csv", header = TRUE) 

# Display the structure of the dataset str(credit_data) 

# Summary statistics of the dataset summary(credit_data) 

# Check for missing values 

missing_values <- colSums(is.na(credit_data)) print(missing_values)# Check the class distribution of the target variable (assuming the target variable is 

named "Class") 

class_distribution <- table(credit_data$Class) print(class_distribution) 

# Visualize the class distribution using a bar plot 

barplot(class_distribution, main = "Class Distribution", xlab = "Class", ylab = 

"Frequency", col = c("green", "red"), legend = c("Non-Fraud", 

"Fraud")) 

# Plot some exploratory data analysis (EDA) plots (assuming V1-V28 are the 

features) 

# For example, histograms of some features for both classes 

ggplot(credit_data, aes(x = V1, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution of V1 

by Class") + xlab("V1") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal() 

ggplot(credit_data, aes(x = V2, fill = factor(Class))) + 

geom_histogram(bins = 30, alpha = 0.5) + ggtitle("Distribution 

of V2 by Class") + xlab("V2") + ylab("Frequency") + 

scale_fill_manual(values = c("green", "red")) + theme_minimal()
