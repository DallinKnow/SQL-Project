# SQL-Project
A case study using SQL from start to finish.  

---

### Other Projects
1. [Data Projects](https://github.com/DallinKnow/Data-Projects)
2. [🐍 Python Project](https://github.com/DallinKnow/Data-Projects/blob/main/python_cyclistic_data_project.ipynb)
3. [🟩 Excel Project](https://docs.google.com/spreadsheets/d/1dxbqZMrVBJT55H9pjrVh-L1SDW77RRZgI2gmVlOtjj8/edit?usp=sharing)

<br>

# 🚲 Cyclistic Case Study
(A case study on a fictional bike rental company named Cyclistic.)

### ❓ Business Question:
How do annual members and casual riders use Cyclistic bikes differently?

<br>

## 🧹 Start/Cleaning
First, aftrer importing the tables for 2025 trips, I started with merging the files.

### Initial Data Audit
#### I used this query to find any null values that I didn't want to keep
<img width="361" height="248" alt="image" src="https://github.com/user-attachments/assets/c3edd218-e56b-42ed-bdd8-5c5181f9d423" />
<br>

#### Query result ⤵️
##### Note: The columns with no Null values were colapsed more to fit the photo
<img width="1950" height="529" alt="image" src="https://github.com/user-attachments/assets/297d961c-ee21-499b-9d53-36244f8410ab" />
<br>
<br>

#### I then found that there were false starts that didn't have an end lat or lng but did hav a start lng and lat.

<br>

#### Instead of Deleting the nulls this first time.  I created a new proxy duplicate, avoiding adding nulls from end_lat and lng.
#### I did this for simplicity, to keep all data in one place and make a place where I can delete values without deleting source raw data.

<br>

<img width="930" height="211" alt="image" src="https://github.com/user-attachments/assets/7b19bbb2-edeb-4f52-8cf7-512e8906e3b4" />









