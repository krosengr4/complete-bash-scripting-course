- When using cat to view a file, sometimes the file will be too large (1000+ lines)
- This makes it near impossible to correctly search this file

--- PAGERS ---
* Pagination: the process of dividing a large dataset into smaller, dsicrete pages for better usability and performance.

- You can use a pager like 'less' to help with this problem (ex: less test.txt)
    - This allows you to use up and down arrows, pg up and pg down, ctrl + f and ctrl + b to scroll through a large file
    - When finished, just hit q and you are back in a clean terminal

- To search for something specific, you can hit / -> type word -> enter
    - Use 'n' and 'shift + n' to go forwards and backwards through each instance
    - Like using ctrl(cmd) + f in a browser

- To get really fancy, here are some examples of using pipelines with less
    - using cat command then piping the stdout to less
        - cat /usr/shared/dict/words | less
    - Piping cat | grep | less to search for instances of pattern
        - cat /usr/shared/dict/words | grep anti | less
        
