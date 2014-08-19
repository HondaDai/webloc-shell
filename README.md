webloc-shell
============

Create Mac OS X web link (webloc) from shell


### Usage

Just add following code to `~/.zshrc` or `~/.bashrc`

```
webloc() {

  echo '<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>URL</key>
	<string>'$2'</string>
</dict>
</plist>' > $1'.webloc'

}
```

or 

You can run `. ./install-zsh.sh` or `. ./install-bash.sh` to install this. :D



### How to use


```
webloc FILENAME WEBLINK
``` 


### Example

```
webloc google http://google.tw
```

