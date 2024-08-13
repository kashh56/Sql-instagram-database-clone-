# Sql-instagram-database-clone-

## Project Overview

This project involves creating a clone of an Instagram-like database to simulate the data structure of an Instagram system. The database includes various tables that represent key components of the Instagram application, such as users, photos, likes, comments, follows, and tags. 

The goal of this project is to demonstrate SQL query capabilities and provide insights into the data through various analyses. This includes answering specific questions related to user behavior, photo engagement, and hashtag popularity.

## Database Schema

The cloned Instagram database includes the following tables:

- **`users`**: Stores information about users.
  - `user_id` (INTEGER, PRIMARY KEY)
  - `username` (VARCHAR)
  - `created_at` (DATE)
  
- **`photos`**: Contains details about photos uploaded by users.
  - `photo_id` (INTEGER, PRIMARY KEY)
  - `user_id` (INTEGER, FOREIGN KEY)
  - `created_at` (DATE)
  - `photo_url` (VARCHAR)
  

- **`likes`**: Records likes on photos.

  - `photo_id` (INTEGER, FOREIGN KEY)
  - `user_id` (INTEGER, FOREIGN KEY)
  - `created_at` (DATE)

- **`comments`**: Contains comments on photos.
  - `comment_id` (INTEGER, PRIMARY KEY)
  - `photo_id` (INTEGER, FOREIGN KEY)
  - `user_id` (INTEGER, FOREIGN KEY)
  - `created_at` (DATE)
  - `comment_text` (TEXT)

- **`follows`**: Represents follow relationships between users.
  
  - `follower_id` (INTEGER, FOREIGN KEY)
  - `followee_id` (INTEGER, FOREIGN KEY)
  - `created_at` (DATE)

- **`tags`**: Stores tags associated with photos.
  - `tag_id` (INTEGER, PRIMARY KEY)
  - `tag_name` (VARCHAR)
  -  `created_at` (DATE)


- **`photo_tags`**: Stores tags associated with photos.
  - `tag_id` (INTEGER, PRIMARY KEY)
  -  `photo_id`

## SQL Queries

Here are some SQL queries that analyze the data in the database:

### 1. Find the oldest user and also the 5 newest users

### 2. -What day of the week do most users register on?

### 4. - Which user has the most liked photo.

### 5. - Calculate average number of photos per user ?


### 6. - What are the top 5 most commonly use hashtags ?

### 7. - Bot Accounts - Find users who have liked every single photo on the site.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact me :

- email: akashanandani.56@gmail.com
- github: kashh56 



