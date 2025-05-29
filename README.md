#Download the dataset using this code

```
import gdown
import zipfile
import os

# Google Drive file ID (Extracted from your link)
file_id = "1ofKeUIZBsinA_IoJGV74mza8yFBGDCJq"

# Destination file name
output = "file.zip"

# Download the zip file
gdown.download(f"https://drive.google.com/uc?id={file_id}", output, quiet=False)

# Extract the zip file
with zipfile.ZipFile(output, 'r') as zip_ref:
    zip_ref.extractall("")

# Remove the zip file after extraction (optional)
os.remove(output)
```
