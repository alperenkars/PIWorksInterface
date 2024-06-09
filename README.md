### PI Works Interface
## User Interface

### Overview
This screen allows administrators to manage users by adding, editing, and enabling/disabling user accounts.

### Initial State
When the User Management screen is first loaded, the following components are displayed:
- A table listing existing users with columns: ID, User Name, Email, and Enabled status.
- A checkbox labeled "Hide Disabled User", possibly above the table.
- A button labeled "+ New User", left next to checkbox.
- An empty form on the right side for adding or editing users.

### UI Components and Behavior

#### Table
- **Columns**: ID, User Name, Email, Enabled
  - The **ID** column displays the ID for each user.
  - The **User Name** column displays the username of each user.
  - The **Email** column displays the email address for each user.
  - The **Enabled** column displays the status of each user in (true/false) format.

#### Checkboxes
- **Hide Disabled User**: 
  - When checked, only users with `Enabled` status set to `true` are shown in the table.
  - When unchecked, all users are shown regardless of their `Enabled` status. (I assume this should be the behavior depending on the given screenshot)

#### Buttons
- **+ New User**:
  - Clicking this button creates an empty form on the right, allowing the admin to enter details for a new user.
- **Save User**:
  - Clicking this button saves the information entered in the form to create a new user or update an existing user.

#### Form Fields
- **Username**: A text input for the user's username.
- **Display Name**: A text input for the user's display name.
- **Phone**: A text input for the user's phone number.
- **Email**: A text input for the user's email address.
- **User Roles**: A dropdown menu to select user roles (Guest, Admin, SuperAdmin).
- **Enabled**: A checkbox to set the user's status as enabled or disabled.

### Form Behavior
- **New User Form**: Initially, the form fields are empty.
- **Edit User Form**: When a user row in the table is clicked, the form is populated with the selected user's details for editing.
- **Validation**: 
  - All fields are required except for the phone number.
  - The email field should have a valid email address format.
- **Save Action**:
  - If the form is valid, clicking "Save User" will save the details and update the user table. (Again, assuming the behavior from the screenshot)
  - If the form is invalid, appropriate error messages will be displayed next to the fields.

Alperen Kars
