# python-code-to-download-udemy-course
This piece of code will allow to download videos from most of website( i did on Udemy.com)

# First step is to download youtube dl exe
https://github.com/rg3/youtube-dl/releases/tag/2018.01.27/

# This will work when you download youtube.dl, then it download all folders and videos in a sequence
youtube-dl -u string@gmail.com -p passwordstring -o "./%(playlist)s/%(chapter_number)s-%(chapter)s/%(autonumber)03d-%(title)s.%(ext)s" https://www.udemy.com/ten-excel-features-every-analyst-should-know/learn/v4/content


# List available formats
youtube-dl -u <username> -p <password> -F -o './videos/%(playlist)s/%(chapter_number)s - %(chapter)s/%(title)s.%(ext)s' https://www.udemy.com/course-name/

# Download the specified format
youtube-dl -u <username> -p <password> -f <desired-format> -o './videos/%(playlist)s/%(chapter_number)s - %(chapter)s/%(title)s.%(ext)s' https://www.udemy.com/course-name/

# Download specific items
youtube-dl <url> --cookies <cookies-filename> --playlist-items "<comma-separated-indices>"

# Skip specific indices
youtube-dl <url> --cookies <cookies-filename> --playlist-start START_NUMBER
