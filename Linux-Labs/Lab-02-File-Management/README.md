# Lab 2 - File Management

## Objective

Learn basic file management commands using the macOS terminal.

## Commands Used

- touch
- cp
- mv
- rm

## Steps Performed

1. First creating a `Cyberlabs` directory followed by both the `Evidence` and `Reports` directories within the `CyberLabs` directory using the `ls` command.
2. Navigated into the `Reports` directory using `cd Reports`.
3. Created a file named `report1.txt` using the `touch report1.txt` command.
4. Created a second file named `report2.txt` using the `touch report2.txt` command.
5. Used `ls` to verify that both files were successfully created.
6. Created a backup copy of `report1.txt` named `backup.txt` using the `cp report1.txt backup.txt` command.
7. Renamed `report2.txt` to `final_report.txt` using the `mv report2.txt final_report.txt` command.
8. Used `ls` to verify that the copied and renamed files were present in the directory.
9. Removed `backup.txt` using the `rm backup.txt` command.
10. Used `ls` to verify that the backup file had been deleted and that only `report1.txt` and `final_report.txt` remained.
11. The final step in this lab was the use of `rm final_report report1.txt` to remove both `.txt` files from the `Reports` directory, followed by `ls` to verify the files were removed.

## Results

Successfully created and organized directories, created files, copied files for backup purposes, renamed files, removed unnecessary files, and verified changes using command-line tools. Demonstrated the ability to manage files throughout their entire lifecycle using the macOS/Linux terminal.

## Screenshots

<img width="550" height="392" alt="image" src="https://github.com/user-attachments/assets/9c449dd7-c17a-44b3-ba5a-476a607281de" />
<img width="552" height="79" alt="image" src="https://github.com/user-attachments/assets/1c959f87-d108-4999-acc6-4c975e680f9b" />

<sub><em>Navigated into the recently created `Reports` directory to perform file management tasks. Created `report1.txt` and `report2.txt` using the `touch` command, verified their creation with `ls`, created a backup copy of `report1.txt` using `cp`, and renamed `report2.txt` to `final_report.txt` using `mv`. The backup file was then removed with `rm backup.txt` and the remaining files were verified using `ls`. The lab concluded by deleting both text files with the `rm` command and confirming the directory was empty.</em></sub>
