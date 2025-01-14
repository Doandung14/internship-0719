-**TTY** (TeleType)

> an Identifier for terminal, not all processes having it 

-**Kernel**

> a heart of Linux, a core of OS

-**`top`**

> show system’s resources usage and processes that consume resources 

-**`htop`** 

> an improved “top”, give n easier-to-understand GUI, and action keys 
to do with processes “F”


-**`df -h`** Show free space on partitions in a readable format

-**`free -g`** Show RAM usage in gigabytes 

-**`pid (process name)`** to find the pid of a process

-**`nice -n ”number” (process name)`** set the nice number for a process 

-**`renice “number” -p (process number)”`** reset the nice number of a process that already started

-**`ps`**

> show processes(from its own terminal by default)

1. `ps -u (an user or users)` processes and program running under an user or under multiple users
2. `ps -a` all except session leader and process that not associate with a terminal
3. `ps -d` all except session leader 
4. `ps -N` all except those that fulfill the specified condition 
5. `ps -C (process name)` filter by a process named “process name”
6. `ps -e -o …,…,….,` filer all process by those fields (...)
7. `ps t` all that associated with this terminal
8. `ps -p` select by pid 
9. `ps – G (RGID)` select by real group name
10. `ps -g` select by EGID
11. `ps w > ps.txt`  you can then examine the output file in a text that support widelines
12. `ps -aux`  show all processes owned by user “x”


-**Kill Process** There’re manyways to kill processes:

1. `killall +name` Ideal for processes that you’ve already knew their exact names and they mustnt in Z or D status
2. adding sigkill to force them terminate immediately : `killall -9 +name`or, you can use: `-sigterm` to gracefully terminate process and let them running some code before they’re killed
3. killall + with confirm : `killall -i +name`
4. kill process that has been running more than marked time : `killall -o **... +name`,this ** characters are minutes are set, and “...” can be “s,m,h,d,w,M,y” , in the other hand use -y for reverse timming
	
=> while youre not sure about an exact name of a process, use pkill + name 