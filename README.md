# Image Downloader

## 1. Introdoction

Crawl and download images using Selenium
Using python3 and PyQt5

## 2. Key features

+ Supported Search Engine: Google, Bing, Baidu
+ Keywords input from keyboard, or input from line seperated keywords list file for batch process.
+ Download image using customizable number of threads.
+ Fully supported conditional search (eg. filetype:, site:).
+ Switch for Google safe mode.
+ Proxy configuration (socks, http).
+ CMD and GUI ways of using are provided.

## 3. Install

### 3.2 Download and setup chromedriver

+ Require Google Chrome Browser or Chromium Browser installed.
+ chromedriver will be install automatically and added in the PATH

~~Download the corresponding version of chromedriver from [here](https://chromedriver.chromium.org/downloads)~~
~~Copy `chromedriver` binary to ${project_directory}/bin/ or add it to PATH.~~

~~3.3 Download and setup phantomjs [deprecated]~~

~~Official phantomjs prebuilt executable can be downloaded from [here](https://bitbucket.org/ariya/phantomjs/downloads)~~
~~Copy `phantomjs` to ${project_directory}/bin/ or add it to PATH.~~

### 3.3 Install python packages

```bash
pip3 install -r requirements.txt
```

## 4. Usage

### 4.1 GUI

Run `image_downloader_gui.py` script to yank GUI:
```bash
python image_downloader_gui.py
```
![GUI](/GUI/GUI.png)

### 4.2 CMD

```bash
usage: image_downloader.py [-h] [--engine {Google,Bing,Baidu}]
                           [--driver {chrome_headless,chrome,phantomjs}]
                           [--max-number MAX_NUMBER]
                           [--num-threads NUM_THREADS] [--timeout TIMEOUT]
                           [--output OUTPUT] [--safe-mode] [--face-only]
                           [--proxy_http PROXY_HTTP]
                           [--proxy_socks5 PROXY_SOCKS5]
                           keywords

## Example
python image_downloader.py  -o /Users/linshan/Downloads/  -n 200 "Face Mask"
```

## License

+ MIT License
+ 996ICU License
