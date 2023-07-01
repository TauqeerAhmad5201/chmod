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
