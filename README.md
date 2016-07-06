# Razercfg-cli

An alternative client for razercfg for my personal use.

## Install

```sh
wget https://raw.githubusercontent.com/janstuemmel/razercfg-cli/master/razercfg-cli
sudo cp razercfg-cli /usr/local/bin
```

## Usage

```sh

usage: razercfg-cli [-h] [-m MOUSE]
                    {mice,profiles,dpimapping,res,freq,led} ...

positional arguments:
  {mice,profiles,dpimapping,res,freq,led}
    mice                shows mice
    profiles            shows and sets profiles
    dpimapping          shows and sets dpi mappings
    res                 shows and sets resolutions
    freq                shows and sets frequency
    led                 shows and sets leds

optional arguments:
  -h, --help            show this help message and exit
  -m MOUSE, --mouse MOUSE


```

# Example

```sh

razercfg-cli led -l GlowingLogo -m static -c FF0000 &
razercfg-cli led -l Scrollwheel -m static -c 0000FF &
razercfg-cli freq -s 1000 &
razercfg-cli res -s 400x400 &

```
