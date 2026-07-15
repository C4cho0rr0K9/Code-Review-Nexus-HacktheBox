The five fantastics Survival Kit of the os library

1. os.getcwd() -> where we are? 
 - The Equivalent en linux is = pwd

Example:

whereWeAre = os.getcwd()
print(f"Exact Coordinates: {whereWeAre})

2. os.listdir() -> It show us everithign there is in the current folder
 - The equivalent in linux is = ls or dir

Example:

print("Escaneando el directorio actual...")
content=os.listdir(".") -> current folder
for item in content
    print(f" |---{conent})

3. os.mkdir() -> Create a new folder
 - The equivalent in Linux is mkdir

Example:
forldername = "security_reports"

 if not os.path.exists(foldername)
     os.mkdir(foldername)
      print(f"[+] The folder '{foldername}' was create")
else:
  print("f[+] The Folder '{foldername}' is already exists, dont create any new folder)


4. os.path.exists() -> check if some folder o archive already exists
   -The equivalent in Linux is test -e

Example:

nameoffile = "config.file"

if os.path.exists(nameoffile):
  print(f"[+] '{nameoffile}' found, Initialiting the system")
else
  print(f"[x] Error, the file '{nameoffile}' is't found".)

5. os.remove() -> Delete a file
   -The equitative linux is rm

Example:
  nameoffile = "temp_data_trash"

  if os.path.exists(nameoffile):
    try:
        os.delete(nameoffile)
        print(f"[x] temporal file '{nameoffile}' deleted successfully")
      exept PermissionError:
        print(f"[-] ERROR: You dont have any permission to delethe the '{nameoffile}' file")
  else:
      print(f"[-] The file '{nameoffile}' dont exists")




                 ███████╗ █████╗ ███╗   ██╗████████╗ █████╗ ███████╗████████╗██╗ ██████╗
                 ██╔════╝██╔══██╗████╗  ██║╚══██╔══╝██╔══██╗██╔════╝╚══██╔══╝██║██╔════╝
                 █████╗  ███████║██╔██╗ ██║   ██║   ███████║███████╗   ██║   ██║██║
                 ██╔══╝  ██╔══██║██║╚██╗██║   ██║   ██╔══██║╚════██║   ██║   ██║██║
                 ██║     ██║  ██║██║ ╚████║   ██║   ██║  ██║███████║   ██║   ██║╚██████╗
                 ╚═╝     ╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝╚══════╝   ╚═╝   ╚═╝ ╚═════╝

         ███████╗██╗██╗   ██╗███████╗    ██╗  ██╗██╗   ██╗████████╗
         ██╔════╝██║██║   ██║██╔════╝    ██║  ██║██║   ██║╚══██╔══╝
         █████╗  ██║██║   ██║█████╗      ███████║██║   ██║   ██║
         ██╔══╝  ██║╚██╗ ██╔╝██╔══╝      ██╔══██║██║   ██║   ██║
         ██║     ██║ ╚████╔╝ ███████╗    ██║  ██║╚██████╔╝   ██║
         ╚═╝     ╚═╝  ╚═══╝  ╚══════╝    ╚═╝  ╚═╝ ╚═════╝    ╚═╝

---

## 🔹 1. `os.getcwd()` — Where are we?
> **Linux equivalent:** `pwd`

```python
whereWeAre = os.getcwd()
print(f"📍 Exact Coordinates: {whereWeAre}")
📂 Output:
📍 Exact Coordinates: /home/user/projects/awesome_app
```

🔹 2. os.listdir() — What's in the folder?
Linux equivalent: ls / dir
 ``python
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
🔹 3. os.mkdir() — Create a new folder
Linux equivalent: mkdir

#Example:
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

🔹 4. os.path.exists() — Does the file/folder exist?
Linux equivalent: test -e
nameoffile = "config.file"

if os.path.exists(nameoffile):
    print(f"[✓] '{nameoffile}' found, initializing the system")
else:
    print(f"[✗] Error: the file '{nameoffile}' was not found")
📂 Output:
[✓] 'config.file' found, initializing the system
🔹 5. os.remove() — Delete a file
Linux equivalent: rm
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
  ╔══════════════════════════════════════════════════════════════╗
  ║   🧠  Remember: import os at the top of your script!        ║
  ║   💡  os.path.join() is your friend for cross-platform paths ║
  ╚══════════════════════════════════════════════════════════════╝
