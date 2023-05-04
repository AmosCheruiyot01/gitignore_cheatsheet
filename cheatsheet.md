# Rules for .gitignore
## here are the general rules for matching patterns in .gitignore files:

| Patterns                           | Explanation/Matches                                        | Examples |
| --------                  | -------------------                                                    | -------- |
| name.file             | All files with the name.file will be ignored                               | /name.file /lib/name.file |
|name                    | All name files, name folders, and files and 
                            folders in any name folder                                               | /name.log, /name/file.txt, /lib/name.|
|*.file                  | All files withe .file extention 	                                         |/name.file /lib/name.file |
|**/name                 | 	All name folders, and files and folders in any name folder               |/name/log.file, /lib/name/log.file, /name/lib/log.file |
|name?.file              |	? matches a single non-specific character                        |	/names.file, /name1.file, /names1.file |
|lib/name.file           | Patterns specifiing files in specific folders are
                                always realative to root (even if you do not start with / )          | /lib/name.file|
|/lib/**/name            |	All name folders, and files and folders in any 
                                name folder within the lib folder.                                    |/lib/name/log.file, /lib/test/name/log.file |
