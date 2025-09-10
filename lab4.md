# 📌 BACKUP



# ✅1.⁠ ⁠backup.sh Script
Create a new file named backup.sh inside your project folder:
<img width="743" height="423" alt="Screenshot from 2025-09-09 14-48-55" src="https://github.com/user-attachments/assets/be86b452-286e-409d-8c24-28b093918ac9" />


# ✅ 2. Make Script Executable
Run the following command once:

chmod 777 backup.sh

# ✅ 3. Testing the script
## 1. Create some samples .txt files:
<img width="780" height="50" alt="Screenshot from 2025-09-09 14-46-10-1" src="https://github.com/user-attachments/assets/0c84c3c0-ce26-41ee-821a-d4a9ed4d75c9" />

## 2. Run the script:

./backup.sh
<img width="754" height="97" alt="Screenshot from 2025-09-09 14-46-43" src="https://github.com/user-attachments/assets/81a1a8ba-78f1-4b08-b2da-2b19140eedb9" />

## 3. Check the backup/folder:

ls backup/
<img width="1108" height="71" alt="Screenshot from 2025-09-09 20-07-30" src="https://github.com/user-attachments/assets/a470ac54-88fd-46de-88c0-8b3c80cfa151" />



# 🔧 LAB4– File & Backup Automation

## Objective
Automate the backup of ⁠ .txt ⁠ files into a ⁠ backup/ ⁠ folder with timestamps in filenames.

---

## 🔧 Script Explanation

1.⁠ ⁠⁠ mkdir -p backup ⁠  
   Creates a folder n".

🔹 3. Using at (One-time Scheduling)
Run a script once at a specific time:

echo "/home/user/backup.sh" "
amed ⁠ backup ⁠ if it does not exist.

2.⁠ ⁠⁠ timestamp=$(date +"%Y%m%d_%H%M%S") ⁠  
   Generates a timestamp (format: YYYYMMDD_HHMMSS).

3.⁠ ⁠⁠ for file in *.txt; do ... done ⁠  
   Loops through all ⁠ .txt ⁠ files in the current directory.

4.⁠ ⁠⁠ basename "$file" .txt ⁠  
   Extracts the file name without extension.

5.⁠ ⁠⁠ cp "$file" "backup/${filename}_$timestamp.txt" ⁠  
   Copies the file into ⁠ backup/ ⁠ with the timestamp appended.

---

## 🔧 Example Run

### Input
Created two ⁠ .txt ⁠ files:

file1.txt
world.txt


### Command
./backup.sh


### Output
Files copied into ⁠ backup/ ⁠ with timestamps:

<img width="592" height="100" alt="Screenshot from 2025-09-09 20-10-08" src="https://github.com/user-attachments/assets/e803f350-d767-4530-8331-c5fd5270a36c" />

### 🛠️ Q1-What is the difference between cp,mv,and rsync?

     ans=cp-Copies files or directories
         rm-Moves or renames files or directories
         rsync-Synchronizes files/directories efficiently


### ✅ Q2-How can you schedule scripts to run automatically?
     

     ans=You can schedule scripts to run automatically using task schedulers built into your operating system.
