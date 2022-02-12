[![windows](https://img.shields.io/badge/Download-Windows-blue?style=for-the-badge&logo=Microsoft)](https://github.com/Mennaruuk/twayback/releases/download/02%2F04%2F2022/twayback.exe)
[![python](https://img.shields.io/badge/Download-Python-red?style=for-the-badge&logo=python)](https://github.com/Mennaruuk/twayback/releases/download/02%2F04%2F2022/twayback.zip)

![screenshot](https://i.imgur.com/oBeqt6V.png)


Finding and downloading deleted Tweets takes a lot of time. Thankfully, with this tool, it becomes a piece of cake! 🎂

Twayback is a portmanteau of *Twitter* and the *Wayback Machine*. Enter your desired Twitter username, and let Twayback do the rest!

## Features
 - Can download some or all of a user's archived deleted Tweets.
 - Lets you extract Tweets text to a text file (yes, even quote retweets!)
 - Allows custom time range to narrow search for deleted Tweets archived between two dates.
 - Differentiates between accounts that are active, suspended, or don't/no longer exist.
 - Lets you know if a target handle's archived Tweets have been excluded from the Wayback Machine.

## Usage
    twayback -u USERNAME [OPTIONS]
    Example: twayback -u jack
    
    -u, --username        Specify target user's Twitter handle
    -from, --fromdate     Narrow search for deleted Tweets *archived* on and after this date
                          (can be combined with -to)
                          (format YYMMDD)
    -to, --todate         Narrow search for deleted Tweets *archived* on and before this date
                          (can be combined with -from)
                          (format YYMMDD)

## Installation
### For Windows only
 1. [Download the latest EXE file.](https://github.com/Mennaruuk/twayback/releases/download/02%2F12%2F2022/twayback.exe)
 2. Launch Command Prompt in the EXE file's directory.
 3. Run the command `twayback -u USERNAME` (Replace `USERNAME` with your target handle).

### For Windows, Linux, and macOS
 1. [Download the latest ZIP file.](https://github.com/Mennaruuk/twayback/releases/download/02%2F12%2F2022/twayback.zip)
 2. Extract ZIP file to a directory of your choice.
 3. Open terminal in that directory.
 4. Run the command `pip install -r requirements.txt`.
 5. Run the command `twayback -u USERNAME` (Replace `USERNAME` with your target handle).


For more information, check out the [Usage](#usage) section above.

## Things to keep in mind
 - Quality of the HTML files depends on how the Wayback Machine saved them. Some are better than others.
 - This tool is best for text. You might have some luck with photos. You cannot download videos.
 - By definition, if an account is suspended or no longer exists, all their Tweets would be considered deleted.
 - Custom date range is not about when Tweets were made, but rather when they were _archived_. For example, a Tweet from 2011 may have been archived today.
