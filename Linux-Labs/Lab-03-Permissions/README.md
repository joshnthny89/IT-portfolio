# Lab 03 - File Permissions

## Objective

I show how to view and modify file permissions in macOS/Linux using the terminal. Show how file permissions help protect sensitive information by controlling who can read, write, and execute files.

## Commands Used

- touch
- ls -l
- chmod 600
- chmod 644

## Steps Performed

1. Created a file named `sensitive.txt` using the `touch` command.
2. Viewed the file's default permissions using `ls -l`.
3. Modified the file permissions to `600` using `chmod 600 sensitive.txt`.
4. Verified the permission changes using `ls -l`.
5. Modified the file permissions to `644` using `chmod 644 sensitive.txt`.
6. Verified the updated permissions using `ls -l`.
7. Modified the file permissions to `777` using `chmod 777 sensitive.txt`.
8. Verified the updated permissions using `ls -l`.
9. Compared the differences between the permission settings and analyzed their security implications.

## Results

Successfully viewed and modified file permissions using the `chmod` command. Demonstrated how permission settings can restrict or allow access to files, helping to protect sensitive data from unauthorized access.

## Permission Breakdown

### Permission 600

- Owner: Read, Write
- Group: No Access
- Others: No Access

**Security Impact:** Restricts file access to the owner only and is commonly used for sensitive files.

### Permission 644

- Owner: Read, Write
- Group: Read Only
- Others: Read Only

**Security Impact:** Allows other users to view the file while preventing them from making changes.

### Permission 755

- Owner: Read, Write, Execute
- Group: Read, Execute
- Others: Read, Execute

**Security Impact:** Commonly used for scripts and directories that need to be accessed by multiple users.

### Permission 777

- Owner: Read, Write, Execute
- Group: Read, Write, Execute
- Others: Read, Write, Execute

**Security Impact:** Provides full access to all users and is generally considered insecure because it can allow unauthorized modifications.

## Screenshot

<img width="498" height="279" alt="image" src="https://github.com/user-attachments/assets/0c8af455-e313-4b00-a767-d3082c4455f4" />


<sub><em>Terminal output showing the creation of a test file, inspection of default permissions using `ls -l`, and modification of file permissions using `chmod`.</em></sub>

## Lessons Learned

File permissions are a critical security control that help protect systems and data. Understanding how to view and modify permissions is essential for system administration, cybersecurity, and incident response activities. 

## Skills Demonstrated

- Linux/macOS Terminal Usage
- File Permission Management
- Principle of Least Privilege
- Security Fundamentals
- Technical Documentation
