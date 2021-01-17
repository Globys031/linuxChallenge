# linuxChallenge
After running the script I take input on how many random strings I want to make. The length of each string is random. I then make a file with a random name tmp.XXX (where XXX is the random part) and set a limit to its size (1MB).
Using a for loop I create the amount of random strings specified. Taking /dev/urandom device node as input I generate a random string (didn't use /dev/random since I heard it takes longer).
After that I sort the file alphabetically while ignoring cases. I then remove all the lines starting with either a or A and output it to a different file named "alteredFile". By comparing the original file with "alteredFile" I find how many lines have been removed.

Note that "alteredFile" gets overwritten when the script is run. However, a new tmp.XXX is created each time
