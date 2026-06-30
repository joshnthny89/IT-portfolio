# Lab 04 - Users & Groups

## Objective

I show how to view user accounts, identify groups, and understand how user and group management controls access to system resources. This lab demonstrates foundational identity and access management (IAM) concepts used in system administration and cybersecurity.

## Commands Used

- whoami
- id
- groups
- dscl, dscl .read/Users
- sudo -l, sudo -v
- users


## Steps Performed

1. Used the `whoami` command to identify the current logged-in user account.

2. Used the `id` command to display the user's UID, GID, and group memberships.

3. Used the `groups` command to identify groups associated with the current user.

4. Used `dscl . list /Users` to query available user accounts stored on the macOS system.

5. Used `dscl . read /Users/[username]` to view detailed account information including user ID, group ID, and shell information.

6. Used `sudo -v` to authenticate administrative privileges.

7. Used `sudo dscl . list /Users` to perform directory queries with elevated permissions.

8. Used `sudo -l` to review commands available to the current user with administrative privileges.

9. Reviewed how user accounts, groups, and administrative permissions influence access control.

## Results

Successfully identified user account information, viewed group memberships, and analyzed how user identity and group assignments affect system access. Demonstrated an understanding of how account management supports security and access control.

## Security Concepts Demonstrated

### Identity and Access Management (IAM)

User accounts and groups help determine who can access resources and what actions they are allowed to perform.

### Principle of Least Privilege

Users should only have the permissions necessary to perform their required tasks, reducing the risk of unauthorized access.

### User Identification

UIDs and GIDs allow operating systems to uniquely identify users and assign permissions accurately.

## Skills Demonstrated

- macOS/Linux User Management
- Group Membership Analysis
- Identity and Access Management Fundamentals
- Command-Line Administration
- Access Control Concepts
- Security Documentation

## Screenshot

<img width="852" height="183" alt="image" src="https://github.com/user-attachments/assets/f529df07-5270-4ff0-baa4-71515d97a817" />

<sub><em>Used the `whoami` command to identify the currently logged-in user account, the `id` command to display the user's UID, GID, and group memberships, and the `groups` command to verify the groups associated with the user account. These commands were used to review user identity and access information on the macOS system.</em></sub>

<img width="853" height="230" alt="image" src="https://github.com/user-attachments/assets/d3fc6cfd-7e50-4369-970a-17c25e552b71" />

<sub><em>Performed user and group enumeration using the `users`, `groups`, and `dscl . list /Users` commands to review active sessions, group memberships, and user accounts configured on the macOS system.</em></sub>

<img width="735" height="211" alt="image" src="https://github.com/user-attachments/assets/f9c50be2-3a81-4887-a7fd-5c0334410ef7" />
<img width="372" height="168" alt="image" src="https://github.com/user-attachments/assets/e9713374-dd5d-4e1c-a48c-8152ac1eb183" />

<sub><em>Used the `dscl . read /Users/[USERNAME]` command to examine user account attributes and identity information stored within macOS directory services. Reviewed account details such as user identifiers, group associations, and configuration settings as part of an identity and access management analysis.</em></sub>

<img width="443" height="287" alt="image" src="https://github.com/user-attachments/assets/31b2aa56-77d1-465d-8c39-9757a410b6d2" />

<sub><em>Authenticated administrative access using `sudo -v` and used `sudo dscl . list /Users` to enumerate local user accounts with elevated privileges, demonstrating how administrators review account information and access controls.</em></sub>

<img width="843" height="208" alt="image" src="https://github.com/user-attachments/assets/48ee9c50-c83c-40c9-9475-f5dc89ad2c98" />

<sub><em>Finished the lab by using `sudo -l` to review available administrative privileges and verify the level of access assigned to the current user account.</em></sub>

## Lessons Learned

Managing users and groups is a fundamental security practice. Proper account organization and permission management help protect systems by ensuring users have appropriate access while preventing unauthorized actions.
