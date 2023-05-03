Use a forward slash (/) to separate directory names. For example, docs/notes will match all files under the notes directory within the docs directory.

Use an asterisk (_) as a wildcard character. For example, _.log will match all files with the .log extension in any directory.

Place a hash (#) or a semicolon (;) at the beginning of a line to create a comment.

Use two asterisks (_) to match any number of directories. For example, docs/_/notes will match all files under any subdirectory named notes under the docs directory.

Use a question mark (?) to match any single character. For example, file?.txt will match file1.txt or file2.txt but not file10.txt.

Use square brackets ([]) to match a single character from a set of characters. For example, [abc].txt will match a.txt, b.txt, or c.txt, but not d.txt.

Use an exclamation mark (!) to negate a pattern. For example, \*.log followed by !important.log will exclude all log files except for important.log.

Patterns that start with a forward slash (/) are considered to be relative to the root directory of the repository. Patterns without a leading slash are considered to be relative to the directory where the .gitignore file is located.

To include a file or directory that is already excluded by a previous pattern, you can use the negation pattern !. For example, logs/\*.log followed by !logs/error.log will exclude all .log files in the logs directory except for error.log.
