# wslopen

**wslopen** is a handy utility for WSL that opens a file or URI in the user's preferred Windows application for files or URIs of that type.

## Installation

Installing or updating locally for the current user:

```sh
mkdir -p ~/.local/bin && wget -O ~/.local/bin/wslopen 'https://github.com/marveloo/wslopen/raw/main/wslopen' && chmod +x ~/.local/bin/wslopen
```

Or globally on the machine:

```sh
sudo wget -O /usr/local/bin/wslopen 'https://github.com/marveloo/wslopen/raw/main/wslopen' && sudo chmod a+x /usr/local/bin/wslopen
```

## Example Usage

```sh
# Open an image file in the default image viewing application on Windows
$ wslopen /tmp/foobar.png

# Edit a text file in Notepad
$ wslopen 'file:///tmp/foobar.txt'

# Open the current folder in Windows Explorer
$ wslopen .

# Visit a webpage in the user's default browser on Windows
$ wslopen 'https://www.example.com/?foo=bar'

# Compose an email to foo in the preferred Windows email client
$ wslopen 'mailto:foo@example.com'
```
## License

**wslopen** is an open-source tool licensed under the [MIT license](/LICENSE).
