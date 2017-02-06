##Basic Unix Command Line Skill

***Note:*** Lines that start with a `$` should be entered on the command line without the  `$`

**1. Download and navigate to the workshop data**

- Click on the top right `Clone or Download` button and download this repository.
- Open your terminal window. On a Mac, this is contained in the Utilities folder within your Applications folder. On Unix, it should be in your Applications folder as well.
- `cd` into the directory that contains the workshop `.zip` file (on a Mac, this is likely to be `~/Downloads`)
- Enter the command `unzip Unix_Hydra_2hr-master.zip`
- Now `cd` into the new `Unix_Hydra_2hr-master` directory

**2. Make a directory and copy your contents into it**

- Make a new directory called `sequences`
- Copy both sequence files into your `sequences` directory
- Change directories into your `sequences` directory
- Now print the path of the directory you are in to the screen

*Hint-to make a directory, user the `mkdir` command and to copy, use the `cp` command*

**3. Viewing file contents**

- Try all four of these commands to examine the file `sequences.fa`
    
    a)  `$ cat sequences.fa`
    
    b)  `$ head sequences.fa`
    
    c)  `$ tail sequences.fa`
    
    d)  `$ less sequences.fa`   (Remember, `q` is quit in less)
    
- Use `less` to *find the sequences* that contains the description EAS20\_8\_6\_1\_5_388 (Type `h` in less for help screen, look for “Search forward…” in the “SEARCHING” section.).
    
- Use `head` to display the first sequence only (first two lines). Type `$ man head` (or Google) to find the option to limit the number of lines `head` displays (man pages open in `less`, use the arrow keys to navigate and `q` to quit).
    
- Use `tail` and wildcard globbing to display the last 10 lines *of the two sequences files* (`sequences.fa` and `sequences.fq`) with one command.

**4. Edit a file with `nano`**

- Open `sequences.fa` with `nano`
- Change some bases in one of the sequences.
- Save and close the file
*Remember in* `nano` *shortcuts are at the bottom of the screen and* `^` *is the control key.*

**5. Create a new text file and delete it**

- `$ nano newfile` If the filename doesn’t exist, an empty document will be opened.
- Enter some text into the file, save it and exit.
- Use one of the text viewing commands we used in Step 5 to view your new file’s contents.
- After viewing your file delete it with the `rm` command