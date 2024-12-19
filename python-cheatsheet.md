### find all files in a folder

```
import os

dir = "directory"
files = [f for f in os.listdir(dir) if os.path.isfile(os.path.join(dir, f))]

```

### read a txt file

```
with open(file_path, 'r') as file:
    line = file.readline().strip()  # Read the first line and strip any whitespace

# Split the line into parts
parts = line.split()
```
