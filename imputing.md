Imputing missing values can be done using various strategies, such as filling with a specific value, using the mean, median, or mode of the column, or using more advanced techniques like interpolation or machine learning models. Here, I'll show a few basic examples using the pandas library.

1. **Filling missing values with a specific value:**

```python
import pandas as pd

# Sample data
data = {
    'Car_Name': ['Toyota', 'Honda', None, 'Ford', 'Chevrolet'],
    'Year': [2010, 2012, 2015, None, 2018],
    'Price': [5000, 7000, 9000, 11000, 13000]
}

# Create DataFrame
car_cleaned1 = pd.DataFrame(data)

print("Original DataFrame:")
print(car_cleaned1)

# Fill missing values with a specific value
car_cleaned1_filled = car_cleaned1.fillna({
    'Car_Name': 'Unknown',  # Fill missing car names with 'Unknown'
    'Year': 2000,           # Fill missing years with a specific year, e.g., 2000
    'Price': car_cleaned1['Price'].mean()  # Fill missing prices with the mean price
})

print("\nDataFrame after filling missing values:")
print(car_cleaned1_filled)
```

2. **Filling missing values with the mean, median, or mode:**

```python
import pandas as pd

# Sample data
data = {
    'Car_Name': ['Toyota', 'Honda', None, 'Ford', 'Chevrolet'],
    'Year': [2010, 2012, 2015, None, 2018],
    'Price': [5000, 7000, 9000, 11000, 13000]
}

# Create DataFrame
car_cleaned1 = pd.DataFrame(data)

print("Original DataFrame:")
print(car_cleaned1)

# Fill missing numeric values with mean
car_cleaned1['Year'].fillna(car_cleaned1['Year'].mean(), inplace=True)
car_cleaned1['Price'].fillna(car_cleaned1['Price'].mean(), inplace=True)

# Fill missing categorical values with mode
car_cleaned1['Car_Name'].fillna(car_cleaned1['Car_Name'].mode()[0], inplace=True)

print("\nDataFrame after filling missing values with mean/mode:")
print(car_cleaned1)
```

3. **Using interpolation to fill missing values:**

```python
import pandas as pd

# Sample data
data = {
    'Car_Name': ['Toyota', 'Honda', None, 'Ford', 'Chevrolet'],
    'Year': [2010, 2012, 2015, None, 2018],
    'Price': [5000, 7000, 9000, 11000, 13000]
}

# Create DataFrame
car_cleaned1 = pd.DataFrame(data)

print("Original DataFrame:")
print(car_cleaned1)

# Interpolate missing numeric values
car_cleaned1['Year'] = car_cleaned1['Year'].interpolate()

# For non-numeric columns, you could fill them with the most frequent value or another strategy
car_cleaned1['Car_Name'].fillna(car_cleaned1['Car_Name'].mode()[0], inplace=True)

print("\nDataFrame after interpolation and filling missing values:")
print(car_cleaned1)
```

In these examples:
- The first snippet demonstrates filling missing values with specific values.
- The second snippet shows how to fill missing numeric values with the mean and categorical values with the mode.
- The third snippet uses interpolation for numeric values and mode for categorical values.

You can choose the appropriate method based on the nature of your data and the importance of maintaining data integrity.