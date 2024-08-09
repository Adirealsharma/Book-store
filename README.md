# Book Stock Management System - README

## Overview

The Book Stock Management System is a command-line application that helps users manage book-related activities, including account creation, book reading, book recommendations, book donations, and book requests. The application also provides an administrative interface for managing the book collection and user information.

## Features

### User Features
1. **Create Account**: Allows new users to create an account by entering their personal information.
2. **Login**: Users can log in to their account using their username and password.
3. **Read a Book**: Users can select and read a book from the available collection.
4. **Book Recommendations**: Provides book recommendations based on the user's reading history.
5. **View Read Books**: Users can view a list of books they have read.
6. **Donate a Book**: Users can donate books to the system.
7. **Request a Book**: Users can request books that are not currently available in the system.
8. **Rate the System**: Users can rate the system on a scale of 0 to 5.
9. **Logout**: Users can log out of the system.

### Administrative Features
1. **Add a Book**: Allows the administrator to add new books to the collection.
2. **View Number of Users**: Displays the total number of users registered in the system.
3. **View User Details**: Shows detailed information about each user.
4. **View Number of Books Donated**: Displays the total number of books donated by users.
5. **View Donated Books**: Shows a list of all books donated by users.
6. **View Requested Books**: Shows a list of all books requested by users.

## Files and Structure

- **cred**: Stores user credentials (username and password).
- **user_info**: Stores user information such as username, name, phone number, address, and email.
- **booksinfo**: Stores information about books available in the system, including the book name and author.
- **bookuhavered**: Tracks books that users have read.
- **rating_info**: Stores user ratings for the system.
- **donate_info**: Records information about books donated by users.
- **request_info**: Records information about books requested by users.

## How to Run

1. Ensure you have Python installed on your system.
2. Place all the files mentioned above in the same directory as the script.
3. Run the script by executing the following command:
   ```
   python book_management_system.py
   ```
4. Follow the on-screen instructions to use the system.

## How It Works

1. **Initialization**: When the script runs, it initializes several CSV files to store data related to users, books, ratings, and more.

2. **Main Program**:
   - The `main()` function is the entry point of the program. It prompts the user to either create a new account or log in as an existing user.
   - Depending on the user's input, different functions are called to handle account creation, login, and various user and administrative actions.

3. **Account Management**:
   - `forcreateaccount()`: Handles the creation of a new user account and stores user credentials.
   - `forlogin()`: Handles user login by validating the username and password against the stored credentials.

4. **Book Management**:
   - `addbook()`: Allows the administrator to add new books to the system.
   - `readabook()`: Allows users to select and read a book from the available collection.

5. **Rating**:
   - `rate()`: Prompts users to rate the system.
   - `ratevalue()`: Calculates and displays the average rating of the system.

6. **Administrative Functions**:
   - `formanager()`: Allows access to administrative features after verifying the administrator key.
   - `main2()`: Provides a menu for administrative tasks such as viewing users, managing books, and viewing requests.

7. **User Session**:
   - `main3()`: Provides a menu for users to choose actions such as reading books, viewing read books, and more.
   - `forlogout()`: Logs out the user and records the logout time.

## Future Enhancements

- Add more functionalities like tracking the due date of borrowed books.
- Implement a graphical user interface (GUI) for better user experience.
- Integrate a database for more efficient data management.

## Contact

For any issues or contributions, please reach out to [adityaforgames03@gmail.com].

