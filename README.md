# README

## SorterFrequency330

### Overview

SorterFrequency330 is a Java program that reads data from a file containing member visit information and identifies the top N most frequent members. Additionally, it provides an outline for a more extensive system with classes representing club members, managers, and a system for managing member data.

### Requirements

To run the Java program, ensure you have the following:

- Java Development Kit (JDK) installed on your system.

### Running the Java Program

1. Clone the repository:

   ```bash
   git clone https://github.com/Isafarii/SorterFrequency330.git
   ```

2. Navigate to the project directory:

   ```bash
   cd SorterFrequency330
   ```

3. Compile the Java program:

   ```bash
   javac Sorter.java
   ```

4. Run the program:

   ```bash
   java Sorter
   ```

### Understanding the Code

The Java program (`Sorter.java`) reads data from a file named "file.txt" and identifies the top N most frequent members based on their visit counts. You can customize the value of `n` to display a different number of top members.

### Extending the System

The code outline proposes a system with classes like `Member`, `Manager`, and `System`. It also provides a Python class (`DataFilters`) with methods to filter members based on visit history and frequency, as well as search functionality.

### Data Filters Implementation

The `DataFilters` class in Python provides methods for:

- `apply_30_days_filter`: Returns members who haven't visited the club in the past 30 days and highlights members nearing their MembershipEndDate.

- `most_frequent_users_list`: Returns a list of the top ten most frequent members sorted by visit frequency.

- `search_members`: Searches for members based on name or MemberID and returns matching members.

### Example Usage

To use the data filters, create a list of `Member` objects and instantiate the `DataFilters` class. Example usage:

```python
all_members = [...]  # List of Member objects
filters = DataFilters(all_members)
filtered_members = filters.apply_30_days_filter()
top_frequent_members = filters.most_frequent_users_list()
search_result = filters.search_members("John Doe")
```

### Contribution

If you would like to contribute to this project, feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/Isafarii/SorterFrequency330).

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
