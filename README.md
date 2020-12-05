# Custom Lightshot server
<a href="https://www.buymeacoffee.com/Cerus" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## What is this?
This is a custom server for the screen shot tool [Lightshot](https://app.prntscr.com/en/index.html).

## How do I install this?
Download the latest build [here](https://github.com/RealCerus/lightshot-server/releases/latest) and run the jar file.

Example command line arguments:
```
java -Xmx100M -jar LightShotServer-VERSION.jar host=example.com port=8080 https=false pageValid=validPage.html pageInvalid=invalidPage.html
```

### Command line options
- `host`: Your host name. (String)
- `port`: Your port. (Integer)
- `https`: Whether to use https or not. (Boolean)
- `pageValid`: File path of the page which will be shown when a user requests to see an existing (valid) image (String)
- `pageInvalid`: File path of the page which will be shown when a user requests to see a non existing (invalid) image (String)
- `logCons`: (Optional) Sets whether connections should be logged or not (Boolean)

## How do I use this (client side)?
1. You need to have the Lightshot tool installed.
2. Open your `hosts` file. (Windows: `%windir%\system32\drivers\etc\hosts`)
3. Add this line: `127.0.0.1 upload.prntscr.com` (replace `127.0.0.1` with the ip of your server)
4. Restart the Lightshot task (and reload your hosts file if needed)
