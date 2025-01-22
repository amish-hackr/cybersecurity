# Environment Enumeration

### Check OS Version

    cat /etc/os-release

### Check current user PATH

    echo $PATH

### Check out environment variables

    env

### Check kernel version

    cat /proc/version

or

    uname -a

### Gather inforamation such as CPU type/version

    lscpu

### Check for existing login shells

    cat /etc/shells

### Check for drives and mount points

    lsblk    # block devices

    lpstat   # attached printers

    cat /etc/fstab    # mount points

### Check network routing tables

    route
    netstat -rn

### Check for domain/internal DNS

    /etc/resolv.conf

### Check arp records

    arp -a

### Check existing users

    cat /etc/passwd
    cat /etc/passwd | cut -f1 -d

### Check existing groups

    cat /etc/group
    getent group sudo      # list users of sudo group

### Hidden files and directories

    find / -type f -name ".*" -exec ls -l {} \; 2>/dev/null | grep htb-student
    find / -type d -name ".*" -ls 2>/dev/null

### Check temporary files

    ls -l /tmp /var/tmp /dev/shm

    