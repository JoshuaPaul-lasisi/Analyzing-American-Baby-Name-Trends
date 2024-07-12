# Baby Names Analysis

This repository contains a comprehensive analysis of baby names data spanning 101 years, from 1920 to 2020. The analysis includes various tasks that explore the popularity, trends, and patterns of baby names in the United States.

## Tasks

1. **Find Consistently Popular Names**:
   - Find names that have been given to over 5,000 babies of either sex every year for the 101 years from 1920 through 2020.
   - Select the first name and the total number of babies that have ever been given that name.
   - Group by first name and filter for names that appear in all 101 years.
   - Order the results by the total number of babies that have ever been given that name, in descending order.

2. **Classify Name Popularity**:
   - Classify each name's popularity according to the number of years that the name appears in the dataset.
   - Select the first name, the sum of babies who've ever been given that name, and the popularity type.
   - Classify names as 'Classic,' 'Semi-classic,' 'Semi-trendy,' or 'Trendy' based on the number of years the name appears.
   - Order the results alphabetically by first name.

3. **Top 10 American Female Names**:
   - Find the ten highest-ranked American female names in the dataset.
   - Select the name rank, first name, and the sum of babies who've ever had that name.
   - Rank the first names by the sum of babies who've ever had that name, aliasing as name_rank and showing the names in descending order.
   - Filter the data to include only results where sex equals 'F'.
   - Limit the results to ten.

4. **Trendy Female Names**:
   - Find a list of first names that meet specific criteria for a friend's baby name search.
   - Select only the first name column.
   - Filter the data for results where sex equals 'F', the year is greater than 2015, and the first name ends in an 'a'.
   - Group the data by first name and order by the total number of babies ever given that first name, in descending order.

5. **Cumulative Olivias**:
   - Find the cumulative number of babies named Olivia over the years since the name first appeared in the dataset.
   - Select the year, first name, number of Olivias in that year, and the cumulative number of Olivias.
   - Use a window function to calculate the cumulative sum of Olivias up to each year.
   - Filter the results to only include data for the name Olivia.
   - Order the results by year from the earliest year Olivia appeared to the most recent.

6. **Maximum Male Names per Year**:
   - Find the year and the maximum number of babies given any male name in that year.
   - Select the year and the maximum number of babies given any one male name in that year, aliasing the maximum as max_num.
   - Filter the data to include only results where sex equals 'M'.

7. **First Name of Maximum Male Babies**:
   - Using the previous task's code as a subquery, find the first name that corresponds to the maximum number of babies given a specific male name in a year.
   - Select the year, the first name given to the largest number of male babies, and the number of babies given that first name.
   - Join the baby_names table to the subquery, matching on both the num and year columns.
   - Order the results by year, starting with the most recent year.

8. **Top Male Names by Year**:
   - Return a list of first names that have been the top male first name in any year, along with a count of the number of years that name has been the top name.
   - Select the first name and a count of the number of years the first name appeared as a year's top name, aliasing this count as count_top_name.
   - Use the code from the previous task as a common table expression.
   - Group by first name and order the results from the name with the most years at the top to the name with the fewest.

## Data and Tools

The analysis is performed on a dataset of baby names from 1920 to 2020, provided by the Social Security Administration. The queries are written in SQL and can be executed in a PostgreSQL database.

## Conclusion

This repository provides a comprehensive analysis of baby name trends and patterns over the past century. The tasks cover a wide range of topics, including identifying consistently popular names, classifying name popularity, exploring top female and male names, and analyzing the cumulative popularity of specific names. The queries and insights generated from this analysis can be valuable for researchers, marketers, and anyone interested in the evolution of baby naming practices in the United States.
