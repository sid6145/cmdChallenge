# cmdChallenge

# print the current working directory
    pwd

# List names of all the files in the current directory, one file per line.
    ls

# There is a file named access.log in the current directory. Print the contents.
    cat access.log

# Print the last 5 lines of "access.log".
    tail -n 5 access.log

# Create an empty file named take-the-command-challenge in the current working directory.

    touch take-the-command-challenge

# Create a directory named tmp/files in the current working directory
    mkdir tmp && cd tmp && mkdir files

# Copy the file named take-the-command-challenge to the directory tmp/files
    cp take-the-command-challenge tmp/files

# Move the file named take-the-command-challenge to the directory tmp/files
    mv take-the-command-challenge tmp/files

# A symbolic link is a type of file that is a reference to another file.
# Create a symbolic link named take-the-command-challenge that points to the file tmp/files/take-the-command-challenge.
    ln -s tmp/files/take-the-command-challenge take-the-command-challenge

# Delete all of the files in this challenge directory including all subdirectories and their contents.
    rm -rf .* *

# There are files in this challenge with different file extensions. Remove all files with the .doc extension recursively in the current working directory.
    find -name "*.doc" -delete

# There is a file named access.log in the current working directory. Print all lines in this file that contains the string "GET".
     grep "GET" access.log 

# Print all files in the current directory, one per line (not the path, just the filename) that contain the string "500".
     grep -lr 500 

# Print the relative file paths, one path per line for all filenames that start with "access.log" in the current directory.
    ls

# Print all matching lines (without the filename or the file path) in all files under the current directory that start with "access.log" that contain the string "500".
    grep -hr 500

# Extract all IP addresses from files that start with "access.log" printing one IP address per line.
    grep ^[0-9.]* -or 

# Count the number of files in the current working directory. Print the number of files as a single integer.
    ls -o|wc -1

# Print the contents of access.log sorted.
    sort *

# Print the number of lines in access.log that contain the string "GET".
    grep "GET" -c * 

# Print the numbers 1 to 100 separated by spaces.
    echo {1..100}

