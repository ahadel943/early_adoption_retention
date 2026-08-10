# **Early Adoption & Retention**
## **One Question Projects — Project 01**

## **Project Overview**
This project examines whether the timing of a user's first interaction with a product feature is associated with their 30-day retention. The analysis focuses on segmenting users based on how early they adopted the feature and comparing retention across these segments.

## **Business Problem**
Product teams need to understand which early user behaviors are associated with long-term engagement. If early adoption of a key feature is linked to higher retention, encouraging users to discover and use that feature earlier could become an opportunity to improve user retention.

## **Project Goal**
Determine whether users who adopt the feature earlier have higher 30-day retention rates than users who adopt it later.

## **Dataset Description**
The project uses three datasets representing user information, feature adoption behavior, and 30-day retention.

**users.csv**<br> 
Contains basic user-level information.

| Column | Description |
| ------ | ----------- |
| `user_id` | Unique identifier for each user |
| `signup_date` | Date the user signed up |
| `country` | User's country |
| `platform` | Platform used by the user |

**feature_usage.csv**<br>
Contains each user's first usage of the analyzed product feature.

| Column | Description |
| ------ | ----------- |
| `user_id` | Unique identifier for each user |
| `feature_name` | Name of the feature |
| `first_used_date` | Date the user first used the feature |
| `days_after_signup` | Number of days between signup and first feature usage |

The `days_after_signup` field is used to classify users into feature adoption timing segments.

**retention.csv**<br>
Contains the 30-day retention status for each user.

| Column | Description |
| ------ | ----------- |
| `user_id` | Unique identifier for each user |
| `retained_30d` | Indicates whether the user was retained after 30 days (1 = Retained, 0 = Not Retained) |

## **Dataset Scope**
The three datasets are linked through user_id. The analysis combines feature adoption timing with 30-day retention to evaluate whether earlier feature adoption is associated with stronger long-term retention.

## **Exploratory Data Analysis**
### **Users Distribution by Country**
![1](./charts/1.png)
* **Egypt** accounts for the largest share of users (**503**), followed by **Saudi Arabia** (**298**) and the **UAE** (**199**).
## **Users Distribution by Platform**
![2](./charts/2.png)
* **Android** is the most common platform with **432** users, followed by **iOS** (**364**) and **Web** (**204**).








































