## Overview

The User Management Screen is designed to allow administrators to efficiently manage user accounts within the system. This document outlines the requirements, UI components, and expected behavior for this screen.

## Requirements

1. **User List:**
   - Display a list of all users with relevant details (ID, User Name, Email, Enable/Disable info (Bool)).
   - Enable sorting and filtering options for easy navigation.
   - Include a checkbox to hide or show disabled users.

2. **User Details Panel:**
   - Allow administrators to edit user details from this panel.
   - Include a button to save changes made to user details.

3. **User Actions:**
   - Provide options to add, edit, and delete users.
   - Confirmation dialog should be displayed before deleting a user.
   - Include a function to add a new user.
   - Include a function to save changes made to user details.

4. **User Roles:**
   - Allow administrators to assign or modify user roles (SuperAdmin, Admin, Guest).
   - Allow SuperAdmin to assign or modify Admin and Guest
   - Allow Admin to assign or modify Guest. 

5. **Search Functionality:**
   - Update the user list dynamically as the search query changes.



## UI Components

### 1. User List

- Display as a table with columns: User ID, Username, Email, Enabled/Disabled info.
- Implement sorting and filtering options.
- Include a toggle to hide or show disabled users.
- Clicking on a user opens the User Details Panel.

### 2. User Details Panel

- Display user details in a clear and organized format.
- Include an "Edit" button to enable administrators to modify user information.
- Changes made in this panel should be reflected in real-time.
- Include a "Save" button to save changes made to user details.

### 3. New User Panel
- Display a panel with a form to input new user details (Username, Display Name, Phone, Email, User Roles, Enabled/disable info).
- Include a toggle to choose User Roles. 
- Include a checkbox for enabled true/false information


### 4. User Actions

- **Add User:**
  - Open New User Panel	   
  - Validate input fields and display relevant error messages.
  - Upon successful addition, update the user list.

- **Edit User:**
  - Open a modal with pre-filled user details for editing.
  - Validate and update user details in real-time.
  - Include a "Save" button to save changes made to user details.

- **Delete User:**
  - Show a confirmation dialog before proceeding.
  - Remove the user from the list upon confirmation.

## Initial State

- Upon loading, display list of users.
- Show relevant user details in the User Details Panel when a user is selected.
- Include an “New User" button for administrators to initiate the user addition process.

