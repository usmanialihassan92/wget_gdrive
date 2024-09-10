# Downloading Large Files from Google Drive using WGET
First get the editor share link of the google drive file.

Open it in the Microsoft Edge and let it start downloading.

Once the downloading start, right click and copy the download link.

Replace the download link in this command line:

curl -L -o large_file.zip "https://drive.usercontent.google.com/download?id={id}&confirm=t&uuid={uuid}"

Explanation of Parameters
-L (for curl): Follow redirects if necessary.
-O (for wget): Save the file with the name specified after -O.
-o (for curl): Specify the output file name directly.
