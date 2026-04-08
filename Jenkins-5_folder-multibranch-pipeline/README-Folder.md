# Hands-on Jenkins-05: Folder

## Hands-On: Working With Jenkins Folders

### 1. Objective

In this hands-on exercise, you will learn what Jenkins folders are, how
to create them, and how to configure folder-level options such as
permissions, credentials, views, and environment variables.

### 2. What Is a Jenkins Folder?

A Jenkins Folder is a container that organizes pipelines, freestyle
jobs, and other folders. It enables better structure, access control,
and grouping.

### 3. Step 1 --- Create Your First Folder

1.  Go to Dashboard → New Item\
2.  Enter a folder name\
3.  Select **Folder**\
4.  Click **OK**

### 4. Step 2 --- Explore Folder Configuration

Folders support: - Description - Folder icons - Credentials -
Permissions - Environment variables

### 5. Step 3 --- Create Items Inside a Folder

Inside a folder, you can create: - Pipelines - Multibranch Pipelines -
Freestyle Jobs - Nested Folders

### 6. Step 4 --- Nested Folder Structure

Folders can contain folders, allowing hierarchical CI/CD structures.

Example:

    Company/
     ├── Backend/
     │     ├── login-mb
     │     └── payment-mb
     └── Frontend/
           └── webapp-build

### 7. Step 5 --- Create Views Inside a Folder

You can create List Views, Dashboard Views, or Build Monitor Views at
folder level.

### 8. Step 6 --- Inheritance Behavior

Folders pass down: - Credentials\
- Environment variables\
- Permissions

### 9. Hands-On Exercise

Create a private git repo `folder-demo` to test credential inheritance.

Your tasks: 
1. Create hierarchy:
    Company/
     ├── Backend/
     │     ├── login-mb
     │     └── payment-mb
     └── Frontend/
           └── webapp-build

2.  Add folder credentials to Backend\
3.  Configure pipelines under Backend\ and configure the freestyle-job under Frontend/ (use `folder-demo` private github repo)
4.  Create a folder-level View\
5.  Validate inheritance

### 10. Summary

Folders keep Jenkins installations: ✔ Clean\
✔ Organized\
✔ Secure\
✔ Maintainable
