# vim-url-opener

https://github.com/sderev/vim-url-opener/assets/24412384/7bee709e-2878-4e7a-a42d-a375fd8959ca

This is **not a plugin**, but a set of Unix filters following the philosophy: "Do one thing and do it well."

It allows you to open URLs in your web browser from Vim. As such, there is no automated installation process. You will need to manually install the scripts and configuration. But don't worry, it's very simple and takes less than a minute.

I created [a small blog post on my website](https://sderev.com/posts/vim-url-opener) that more or less repeats what's written here, but with more details.

## Usage

To open a URL in your web browser, just place the cursor near the URL and press `gx`. There is no need to have your cursor exactly under the URL.
You can customize the keybind, but it uses `gx` by default.

## Get the Files

**Either by cloning the repository:**

```bash
git clone https://github.com/sderev/vim-url-opener.git
```

**Or by downloading the files directly:**

```bash
curl -O https://raw.githubusercontent.com/sderev/vim-url-opener/main/scripts/extract_nearest_url && \
curl -O https://raw.githubusercontent.com/sderev/vim-url-opener/main/scripts/add_this_to_your_vimrc.txt && \
curl -O https://raw.githubusercontent.com/sderev/vim-url-opener/main/scripts/brave
```

## Installation and Configuration

1. Copy the `extract_nearest_url` script to a directory in your `PATH`. For example: `~/usr/local/bin`.
1. Copy the `brave` script to a directory in your `PATH`.
1. Edit the `brave` script and replace the path to your own web browser.
    * Rename the script to match the name of your web browser.
    * You will also now be able to open URLs in your web browser from your terminal: `brave https://example.com`.
1. Add the content of `add_this_to_your_vimrc.txt` to your `.vimrc`.
    * Change the `brave` command to the name of the script you created in step 3.
    * Change the keybind if you want to use something other than `gx`.

**That's it.**
