The hash data is stored in a CSV in /tmp and is named 'hashed_values.csv'.

If that files exsists, then running ./hash.py will hash all the files on your file system, compare to what is in hashed_values.csv, and print out the differences. 

If the baseline file does not exist, then running ./hash.py will hash all the files on your file system and save the results in /tmp/hashed_values.csv
