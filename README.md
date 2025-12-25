# zed-hackatime

this is a fork of [zed-wakatime](https://github.com/wakatime/zed-wakatime) that should work better with [hackatime](https://hackatime.hackclub.com/)!

## Install
Search for "wakatime" in the "Extensions" page and click "Install".
![type install](./images/install.png)

## Configuration
In order to authenticate with the wakatime-cli, the language server needs to know your API token.
Here are two ways to set the lsp.

### WakaTime configuration file
Create a file named `.wakatime.cfg` in your $HOME directory.
```toml
[settings]
api_key = your-api-key
```
Go through up [wakatime-cli](https://github.com/wakatime/wakatime-cli/blob/develop/USAGE.md)'s documentation for more options.

### Zed settings file
Open Zed's settings file, then add your api key.
```json
"lsp": {
  "wakatime": {
    "initialization_options": {
      "api-key": "Your api key"
    }
  }
}
```

## Note
This plugin has been thoroughly tested only on macOS. If you encounter any issues on other systems, please submit an issue or a pull request.
