# idea-cli
A lightweight command-line tool for capturing notes without breaking flow in Linux/WSL.

## Global installation with curl
```bash
sudo curl -fsSL https://raw.githubusercontent.com/erosche/idea-cli/main/idea \
  -o /usr/local/bin/idea

sudo chmod +x /usr/local/bin/idea
```

## Usage
After installation move into your project root. In bash or WSL run `idea init`. this will create a .idea file in your root directory, and create an IDEA.md file also in your root directory.  

Run `idea 'YOUR IDEA HERE'` to log your ideas to IDEA.md. You can also run `idea` without quotes. E.g. `idea create chron job for data ingest`.  

idea-cli will anchor any log activity to any root project with a .idea file. If you run `idea 'MY IDEA'` and no .idea file is found in the current directory or a parent directory, then the your text  will be logged to a $HOME/.idea.log file.
