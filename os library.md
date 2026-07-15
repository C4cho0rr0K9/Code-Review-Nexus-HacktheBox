## 🔹 1. `os.getcwd()` — Where are we?
> **Linux equivalent:** `pwd`

### Example:

```python
whereWeAre = os.getcwd()
print(f"📍 Exact Coordinates: {whereWeAre}")
📂 Output:
📍 Exact Coordinates: /home/user/projects/awesome_app
```

## 🔹 2. os.listdir() — What's in the folder?
> **Linux equivalent:** ls / dir

### Example:
 ```python
print("🔍 Escaneando el directorio actual...")
content = os.listdir(".")  # current folder
for item in content:
    print(f"  ├── {item}")
📂 Output:
🔍 Escaneando el directorio actual...
  ├── main.py
  ├── config.json
  ├── assets/
  ├── README.md
  └── .gitignor

```
###🔹 3. os.mkdir() — Create a new folder
> **Linux equivalent:** mkdir

### Example:

```python
foldername = "security_reports"

if not os.path.exists(foldername):
    os.mkdir(foldername)
    print(f"[✓] The folder '{foldername}' was created")
else:
    print(f"[✓] The folder '{foldername}' already exists, skipping")
📂 Output:
[✓] The folder 'security_reports' was created

```

##🔹 4. os.path.exists() — Does the file/folder exist?
> **Linux equivalent:** test -e

### Example:

```python
nameoffile = "config.file"

if os.path.exists(nameoffile):
    print(f"[✓] '{nameoffile}' found, initializing the system")
else:
    print(f"[✗] Error: the file '{nameoffile}' was not found")
📂 Output:
[✓] 'config.file' found, initializing the system
``` 

## 🔹 5. os.remove() — Delete a file
> **Linux equivalent:** rm

### Example:

```python
nameoffile = "temp_data_trash"
if os.path.exists(nameoffile):
    try:
        os.remove(nameoffile)
        print(f"[✗] Temporal file '{nameoffile}' deleted successfully")
    except PermissionError:
        print(f"[-] ERROR: You don't have permission to delete '{nameoffile}'")
else:
    print(f"[-] The file '{nameoffile}' does not exist")
📂 Output:
[✗] Temporal file 'temp_data_trash' deleted successfully

```
