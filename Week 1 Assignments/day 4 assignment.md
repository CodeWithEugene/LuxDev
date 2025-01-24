# Week 1 Day 4 Assignment

## Absolute Deviation Mean using a For Loop and a Function

To calculate the absolute deviation mean, you can use the following function:

```python
# Function to calculate the absolute deviation mean
def absolute_deviation_mean(data):
    # Calculate the mean of the data
    mean = sum(data) / len(data)
    # Calculate the absolute deviations from the mean
    absolute_deviations = [abs(x - mean) for x in data]
    # Return the mean of the absolute deviations
    return sum(absolute_deviations) / len(data)

# Example usage of the absolute deviation mean function
my_list = [10, 20, 30, 40, 50]
adm = absolute_deviation_mean(my_list)
print(f"Absolute Deviation Mean: {adm}")
```

## Report Writing: Percent Order

When writing a report, it is common to start from the largest percent and work down to the smallest percent. This helps to highlight the most significant data first.

## Finding Different Percentiles of a List without Using Libraries

```python
# Function to calculate the percentile of a list without using libraries
def percentile(data, percentile_rank):
    # Sort the data
    data.sort()
    # Calculate the index for the given percentile rank
    index = (percentile_rank / 100) * (len(data) - 1)
    lower = int(index)
    upper = lower + 1
    weight = index - lower
    # Return the value at the calculated index
    if upper >= len(data):
        return data[lower]
    return data[lower] * (1 - weight) + data[upper] * weight

# Example usage of the percentile function
my_list = [10, 20, 30, 40, 50]
percentile_25 = percentile(my_list, 25)
percentile_50 = percentile(my_list, 50)
percentile_75 = percentile(my_list, 75)
print(f"25th Percentile: {percentile_25}")
print(f"50th Percentile: {percentile_50}")
print(f"75th Percentile: {percentile_75}")
```