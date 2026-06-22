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

<img width="853" height="179" alt="image" src="https://github.com/user-attachments/assets/ad0d415a-60d4-40c8-8087-57c69b145763" />


<sub><em>Terminal output showing user identification, account details, group memberships, and system user information using macOS command-line tools.</em></sub>

## Lessons Learned

Managing users and groups is a fundamental security practice. Proper account organization and permission management help protect systems by ensuring users have appropriate access while preventing unauthorized actions.
