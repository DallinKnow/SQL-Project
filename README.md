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
I did this for simplicity, to keep all data in one place and make a place where I can delete values without deleting source raw data.

<br>

<img width="930" height="211" alt="image" src="https://github.com/user-attachments/assets/7b19bbb2-edeb-4f52-8cf7-512e8906e3b4" />

<br>

#### Checked nulls again
<img width="889" height="433" alt="image" src="https://github.com/user-attachments/assets/29bc2ba2-f903-4272-83aa-f697e676d4d4" />

<br>

#### Query result ⤵️
<img width="1667" height="82" alt="image" src="https://github.com/user-attachments/assets/f86997a2-bc32-4e14-9f0e-66bfa7debe51" />

<br>

#### ❌ Null values ❌ found in start and end station ID and Names.  
Could be bikes that start and end just not at stations or start at a station and end outside of one, but rides are still not false starts.










