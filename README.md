### README

# Dynamic Dictionary Application

## Overview

The Dynamic Dictionary Application allows users to manage multiple dictionaries with translation capabilities. The application supports two roles: Admin and User. Admins can create new dictionaries, add, remove, update words, and manage admin accounts. Users can view existing dictionaries and get translations of words.

## Features

### Admin Role
- **Admin Login**: Admins must log in with a valid username and password.
- **Create New Dictionary**: Admins can create new dictionaries by specifying language pairs (e.g., "eng ru").
- **Add New Word**: Admins can add new words to existing dictionaries.
- **Remove Word**: Admins can remove words from existing dictionaries.
- **Update Word**: Admins can update the translation of words in existing dictionaries.
- **Add New Admin**: Admins can add new admin accounts.
- **Show All Admins**: Admins can view all admin accounts along with their login and password.

### User Role
- **View Dictionaries**: Users can view a list of available dictionaries.
- **Get Translation**: Users can get translations of words in the specified dictionaries.

## File Structure

### Source Files
- **Main.java**: Entry point of the application. Handles role selection and invokes appropriate menus.
- **Menu.java**: Contains methods for admin and user menus, admin login, and admin management.
- **Methods.java**: Contains methods for dictionary management (creation, word addition, removal, and updating).

### Data Files
- **admins.txt**: Stores admin login credentials in the format `login=password`.
- **dictionaries.txt**: Stores file paths of all created dictionaries.

### Dictionary Files
- Named based on language pairs (e.g., `engru.txt`), these files store words and their translations in the format `word=translation`.

## How to Use

1. **Run the Application**: Start the application by running the `Main` class.
2. **Select Role**: Enter `1` for Admin or `2` for User.
3. **Admin Actions**:
   - Log in with admin credentials.
   - Choose from the admin menu options to manage dictionaries and admin accounts.
4. **User Actions**:
   - Choose from the user menu options to view dictionaries and get translations.

## Admin Management

Admins can manage other admin accounts through the admin menu. Admin credentials are stored in `admins.txt`. To manually add admins, add a line in the format `login=password` to `admins.txt`.

## Dictionary Management

Dictionaries are stored in separate files named based on language pairs (e.g., `engru.txt`). These files can be manually edited if needed, but it is recommended to use the provided admin menu options for consistency.

## Dependencies

- Java 8 or higher
- No external libraries required

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
