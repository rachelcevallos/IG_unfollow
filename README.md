### IG_unfollow

IG_unfollow is a Python script that helps you identify users on Instagram whom you are following, but who do not follow you back.

#### How it Works

IGUnfollow2 parses the HTML of your "following" and "followers" pages on Instagram, extracts the usernames, and then compares the two lists to identify users whom you follow, but who do not follow you back.

#### Usage

1. **Download the HTML Files**: Navigate to your Instagram profile, click on the "Following" and "Followers" tabs, and save the HTML of both pages to your computer. To do this, open your Instagram profile in your browser. Once you've clicked on "Followers," scroll down the window that opens to load all your followers. After doing this, press Ctrl-Shift-I to open the HTML code inspection window. Right-click on the <html> tag at the top and select "Edit as HTML". Then, copy everything (for example with Ctrl-A and Ctrl-C) and paste the content into the file called "followers.html". To paste into "followers.html", open this file with any text editor, such as Notepad. Repeat the procedure for the "Following" section.

3. **Run the Script**: Execute the `main.py` script and provide the paths to the HTML files as arguments.

    ```bash
    python main.py following.html followers.html
    ```

4. **Review the Results**: The script will output the usernames of users you follow but who do not follow you back.

#### Requirements

- Python 3.x
- BeautifulSoup4

#### Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

#### License

[MIT](https://choosealicense.com/licenses/mit/)

