# Template Automation Testing for Web Application

[![Python](https://img.shields.io/badge/Python-2.7.10-lightgrey.svg)](https://www.python.org/)
[![Selenium](https://img.shields.io/badge/selenium-3.6.0-lightgrey.svg)](http://www.seleniumhq.org/)
[![PhantomJS](https://img.shields.io/badge/PhantomJS-2.1.1-lightgrey.svg)](http://phantomjs.org/)
[![ChromeDriver](https://img.shields.io/badge/ChromeDriver-2.33-lightgrey.svg)](https://sites.google.com/a/chromium.org/chromedriver/)
[![Firefox](https://img.shields.io/badge/geckodriver-v0.19.0-lightgrey.svg)](https://github.com/mozilla/geckodriver/releases)
[![OperaDriver](https://img.shields.io/badge/OperaDriver-2.30-lightgrey.svg)](https://github.com/operasoftware/operachromiumdriver/releases)

## [WIKI](https://github.com/damarmustikoaji/seleniumwebdriver/wiki)

## Requirements
- Python >= 2.7.10
- Selenium webdriver >= 3.6.0

```
$ pip install -r requirements.txt
```

## Driver/Browser
- PhantomJS >= 2.1.1
- ChromeDriver >= 2.33
- Firefox/geckodriver >= v0.19.0
- OperaDriver >= 2.30

## Command Arguments
```
$: python Test.py <email> <password> <url> <browser>
```
```
EX$: python Test.py test@gmail password123 http://google.com PhantomJS
```

![alt text](https://github.com/damarmustikoaji/seleniumwebdriver/blob/master/run.gif "Command Arguments")


#### Note Browser :
- Browser = PhantomJS / Chrome / Firefox / Mobile / Default: Chrome
- Mobile : with iPhone 5 Chrome emulator
- Path : ```driver/_file driver_```
```
EX : webdriver.Chrome(executable_path='driver/chromedriver')
```

## Install Virtualenv
- Install
```
$ sudo pip install virtualenv
```
- Create virtualenv
```
$ virtualenv .env
$ source venv/bin/activate
$ deactivate
```
- Reference
- https://dehamzah.com/web/pip-dan-virtualenv-di-python/


## Install PhantomJS
- Install Required Packages
```
$ sudo apt-get update
$ sudo apt-get install build-essential chrpath libssl-dev libxft-dev
$ sudo apt-get install libfreetype6 libfreetype6-dev libfontconfig1 libfontconfig1-dev
```
- Install PhantomJS
```
$ wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-linux-x86_64.tar.bz2
$ tar xvjf phantomjs-2.1.1-linux-x86_64.tar.bz2 -C /usr/local/share/
```

```
$ sudo ln -s /usr/local/share/phantomjs-x.y.z-linux-x86_64/ /usr/local/share/phantomjs
$ sudo ln -s /usr/local/share/phantomjs/bin/phantomjs /usr/local/bin/phantomjs
```

- Verify
```
$ phantomjs --version
```
- Reference
- https://tecadmin.net/install-phantomjs-on-ubuntu/
- http://attester.ariatemplates.com/usage/phantom.html
