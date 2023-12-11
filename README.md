# Creating-Groups-and-Users-
Creating Groups and Users: step by step tutorial
Certainly! Here's a step-by-step tutorial to accomplish the tasks you've mentioned:

### Creating Groups and Users:

#### Step 1: Create the "Accounting" Group and Add User "bob"

Create the "accounting" group:
```bash
sudo groupadd accounting
```

Create the user "bob" and add them to the "accounting" group:
```bash
sudo useradd -m bob
sudo usermod -aG accounting bob
```

#### Step 2: Create the "Production" Group and Add User "sophia"

Create the "production" group:
```bash
sudo groupadd production
```

Create the user "sophia" and add them to the "production" group:
```bash
sudo useradd -m sophia
sudo usermod -aG production sophia
```

#### Step 3: Create the "Admin" Group and Add User "noe"

Create the "admin" group:
```bash
sudo groupadd admin
```

Create the user "noe" and add them to the "admin" group:
```bash
sudo useradd -m noe
sudo usermod -aG admin noe
```

### Viewing User and Group Information:

#### Step 4: Check User and Group Information

The file that holds user information is `/etc/passwd`, and the file that holds group information is `/etc/group`.

To view the user names and the groups they belong to, you can use these commands:

```bash
# To display user names and their IDs
cat /etc/passwd

# To display group names and their IDs
cat /etc/group
```

### Additional Notes:
- The `-m` flag with `useradd` ensures that a home directory is created for each user.
- The `-aG` flag with `usermod` appends the user to the specified group without removing them from their existing groups.

Remember, for security and best practices, always assign appropriate permissions and access rights to users and groups according to your system requirements.
