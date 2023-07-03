# chmod
chmod - change mode

### Different permission examples: 
The chmod command uses a symbolic or numeric mode to specify the permissions to be set. Here's an explanation of the different permissions and how they can be assigned using chmod:

### Numeric Mode:

    The numeric mode represents permissions using a three-digit octal number: xyz.
    x represents the permission for the owner, y for the group, and z for others.
    Each digit can be calculated by adding the values of the following permissions:
        Read (r): 4
        Write (w): 2
        Execute (x): 1
    For example, chmod 755 filename sets the owner to have read, write, and execute permissions (4+2+1 = 7), while the group and others have read and execute permissions (4+1 = 5).
    
### Symbolic Mode 

    The symbolic mode uses a combination of letters and symbols to specify permissions.
    u represents the owner, g represents the group, o represents others, and a represents all (u+g+o).
    + adds permissions, - removes permissions, and = sets the permissions explicitly.
    The basic permission letters are:
        Read (r)
        Write (w)
        Execute (x)
        
 ###   Additional symbolic notations:

    Setuid (s): Allows a file to be executed with the permissions of the file's owner.
    Setgid (s): Allows a file to be executed with the permissions of the file's group.
    Sticky bit (t): When set on a directory, only the owner of a file can delete or rename it.

For example:

    chmod u+x filename adds execute permission for the owner.
    chmod go-rwx directory removes read, write, and execute permissions for the group and others.
    chmod a=rw file.txt sets read and write permissions for all (owner, group, and others), removing execute permission if it was set.
 
