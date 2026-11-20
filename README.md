# Project 5: Secure Linux Server Permissions

## Objective
Implement user-based access restrictions on a Linux server using users, groups, and file permissions.

## Implementation
1. Created two users: `p5alice` and `p5guest`.
2. Created a Linux group named `p5team`.
3. Added `p5alice` to `p5team`.
4. Created a protected directory `/srv/project5-secure`.
5. Assigned ownership to `root:p5team`.
6. Configured directory permissions as `2770` and file permissions as `660`.

## Testing
- **Allowed read:** `p5alice` can read the protected file.
- **Allowed write:** `p5alice` can modify the protected file.
- **Denied read:** `p5guest` cannot read the protected file.
- **Denied write:** `p5guest` cannot create files inside the protected directory.

## Result
Successfully implemented Linux user-based access control using file ownership, group membership, and permission restrictions.

## Conclusion
The project demonstrates the principle of least privilege by granting access only to authorized users.

