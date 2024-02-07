**How to create a VM in VMWare Workstation**

This documentation provides a step-by-step guide on creating a virtual
machine (VM) with a Linux server operating system using VMware
Workstation.

VMware Workstation is a popular virtualization platform that allows you
to run multiple operating systems on a single host machine.

To create a virtual machine, firstly you need 2 things,

1.  A workstation - To create and use a virtual machine

2.  The Server or any operating system that you want to setup on your
    "Virtual Machine".

You can download the workstation and server from their respective
websites available online.

I used ubuntu server for my Virtual machine, I downloaded my server and
VMWARE Workstation from the following websites.

VMware - https://www.vmware.com/in/products/workstation-player.html

Ubuntu - <https://ubuntu.com/download>

After downloading and installing, follow the steps mentioned below to
create a VMware workstation.

**Step1**: Open the VMware Workstation player, then click
on Create a new virtual machine as shown below.

![](/media/image1.png)

**[Step 2**: A pop-up Window will appear infront of you,
select/browse the .iso file downloaded from the ubuntu website and click
on
next.![](/media/image2.png)

![](/media/image3.png)

**Step 3**: Name your new virtual machine as per your
requirement.

![](/media/image4.png)

**Step 4**: Specify the disk capacity for your virtual
machine.![](/media/image5.png)

**Step 5**: Your new virtual machine is almost ready at
this point, this dialogue box shows the essential properties of our
virtual machine, if you like you can customize your hardware as per your
preference just by clicking on customize hardware button.

![](/media/image6.png)

Your Virtual Machine is ready, now you have to install ubuntu in your
virtual machine.

After clicking on finish, this screen will appear infront of you to
install ubuntu server on your VM. Select the option and click on enter
to install Ubuntu Server.

![](/media/image7.png)

**Installing Ubuntu on your virtual machine.**

1.  Select the required language by navigating using up and down arrow
    keys and using enter key to select the required option.

![](/media/image8.png)

2.  Similarily, select the keyboard layout.

![](/media/image9.png)

3.  Choose the base for the installation, here we choose Ubuntu Server
    and then select \[Done\].

![](/media/image10.png)

4.  After choosing the server, now we have to Configure the network
    Connections for our VM. Configure the network settings to ensure
    connectivity. In my case, the system automatically detected the
    Network configurations. If it doesn't then you have to setup that
    manually. Select \[Done\] after
    completing.![](/media/image11.png)

5.  Next step is to configure proxy; if you need to use a HTTP proxy to
    access to the outside world, enterteh proxy information. Otherwise
    leave it blank and proceed.

![](/media/image12.png)

6.  If you use an alternative mirror on Ubuntu, enter its details or
    wait for the mirror location to pass
    tests.
![](/media/image13.png)

7.  Configure a Guided Storage Layout or you can create a custom
    according to your requirements. Then select \[Done\].

![](/media/image14.png)

8.  Check the storage Configuration and proceed.

![](/media/image15.png)

9.  Now setup your name, Server's name, Username and your password to
    login and access your data. Servers name is the name which it uses
    to talk to other
    computers.![](/media/image16.png)

Check the below image for reference:
![](/media/image17.png)

After completing select \[Done\]

10. Then a screen will appear stating SSH Setup, you can choose to
    install openSSH server to enable secure remote access to your sever.
    After that select \[Done\].

![](/media/image18.png)

11. Next page will show all the featured Server Snaps, you can edit it
    as per your preferenece if you like to select or deselect any
    packages. I would recommend to just let it be on default and select
    \[Done\].

![](/media/image19.png)

12. The Systm will start installing, you can view the full log just by
    selecting

\[view full
log\].![](/media/image20.png)

13. After completion of installing, you will get the option to reboot
    the VM. Select the option.
    ![](/media/image21.png)

14. After rebooting, you will get the following page.

![](/media/image22.png)

15. Use your Creditinals that you created earlier in **[step
    3** to login into your server.

![](/media/image23.png)

16. After logging in you will see a welcome page with a few system
    information displayed, now you can run commands and do whatever you
    like on your new Virtual Machine. Your VM is now ready to use.

![](/media/image24.png)

Here are some Linux Commands:

1.  pwd -- print the current working directory.

> ![](/media/image25.png)

2.  ls -- List the files and directories in the current directory.

1.  Ls -l -- lists the files and directories in a detailed form.

2.  Ls -al -- lists the files and directories along with the hidden
    files.

> ![](/media/image26.png)
>
> ![](/media/image27.png)

3.  cd -- change the current directory.

> ![](/media/image28.png)

4.  cd ../ - This command is used to go a folder or directory back from
    the current directory.

> ![](/media/image29.png)

5.  mkdir - create a new directory.

> ![](/media/image30.png)

6.  rmdir -- remove a directory.

> ![](/media/image31.png)

7.  Touch -- create a file.

> ![](/media/image32.png)

8.  Rm -- remove/delete any file

![](/media/image33.png)

9.  Vim -- vim command is used to edit or insert in your crested files.

> ![](/media/image34.png)
>
> Press i to insert into your files
>
> ![](/media/image35.png)

> After you finish inserting pres esc then enter :wq to save and exit,
> :q to quit, :q! to to force quit without save.

10. Cat \>\> filename -- to add new content to an existing file.

> ![](/media/image36.png)

After adding press ctrl + d. Ctrl + d is used to indicate the end of
your input.

11. cp -- used to copy files.

Use -- cp "filename to copy" "destination"

> ![](/media/image37.png)

12. mv -- move any file.

> ![](/media/image38.png)

13. man -- this command stands for manual, it shows us in detail about
    any command we use in linux, for example if we type man ls then it
    shows all related commands to ls. Press q to get back to your
    terminal.

> ![](/media/image39.png)

14. chmod -- allows us to edit permissions of a directory.

> ![](/media/image40.png)

First we type ls -lart, to view the current permissions of any files or
directories.

This are the current permissions allowed, we can change them using chmod
command.

\# The first digit represents the owner of the file/directory

\# The second digit represents the group that the file/directory belongs
to

\# The third digit represents all other users

\# 0 (no permission)

\# 1 (execute only)

\# 2 (write only)

\# 3 (write and execute)

\# 4 (read only)

\# 5 (read and execute)

\# 6 (read and write)

\# 7 (read, write, and execute)

![](/media/image41.png)

15. htop - an interactive process viewer and system monitor

> ![](/media/image42.png)

16. tar - create or extract compressed archive files

\# x: extract files from an archive

\# t: list the contents of an archive

\# r: append files to an existing archive

\# z: use gzip compression

\# j: use bzip2 compression

\# cf: create file

#xf: extract file

tar cf archive.tar file1 file2 file3

![](/media/image43.png)

17. gzip -- compress files

![](/media/image44.png)

18. gunzip -- decompress files

![](/media/image45.png)

19. ssh - connect to a remote server securely

ssh username@server_address

20. ps - display information about running processes.

> ![](/media/image46.png)

21. passwd -- change password for a user.

> ![](/media/image47.png)

22. date - display or set the system date and time

> ![](/media/image48.png)

23. uname - display system information

> ![](/media/image49.png)

24. whoami - display the current user name

> ![](/media/image50.png)

25. echo - display text or variables to the console

![](/media/image51.png)

26. locate - locate any file on the system

![](/media/image52.png)

27. clear -- clears the terminal

![](/media/image53.png)

28. history - display a list of previously executed commands.

> ![](/media/image54.png)

29. df - display disk space usage

![](/media/image55.png)

30. du - display disk usage by file or directory

> ![](/media/image56.png)



