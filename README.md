# betterm

Like *rm*, but better.

Ever accidentally deleted something? Me too. Unfortunately, if one uses the *rm* command it can be quite difficult to retrive lost data. *betterm* arose from the ashes that were once my home folder, in order to save others from similar disasters. 


### How it works

*betterm* uses mv instead of rm to delete files. It simulates moving a file or folder to the trash, so if you delete the wrong thing, it is no big deal. Simply remove it from the trash, brush off any pieces of actual garbage or those coffee grinds you should have composted, and get back to what you were doing.



### Installation

Download bettrm and note the location it was downloaded to. Open terminal and run these commands. Make sure to replace */path/to/betterm* with the path to *bettrm*


```bash
mkdir ~/shell_scripts
mv /path/to/betterm ~/shell_scripts/betterm
chmod 777  ~/shell_scripts/betterm
echo >> ~/.bash_profile; echo 'alias rm="~/shell_scripts/betterm"' >> ~/.bash_profile
source ~/.bash_profile
```

### Usage

If you followed the installation guide, you should be able to use it the following ways:

```bash
rm folder_name
rm file_name
rm path
rm path/file
```

Please test to make sure it's installed properly by deleting something unimportant! I recommend trying this:
```bash
echo test >> test.txt
rm test.txt
```
If installed correctly, you should see output informing you that *betterm* was used.

![Alt text](./demo.png?raw=true "Title")

License
----

MIT
