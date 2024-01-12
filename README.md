# MerismaCapture - dividend capture automation tool

## Description

The aim of a Dividend Capture Algorithm (DCA) is to identify a series of *quality stock dividends, their derivative “put” having an expiration date a few days prior to the ex-dividend date, and their derivative “call” having an expiration date after the ex-dividend date.

The idea is to sell the put that expires days prior the ex-dividend date for which we are paid a premium (x), take possession of the stock shares and collect the dividend (y), after the ex-dividend date, we conclude the transaction by selling a covered call (z), for which we are paid a premium, calling away our shares and exiting our position. Our return is x+y+z.

*quality = we are OK with all outcomes


## Getting Started

### Installing

* Upon cloning repo run `pip install -r requirements.txt` to install all requirements.
* Run `jupyter notebook` to open jupyter in browser.

Everything is installed and you should be able to navigate to the notebooks.

### Executing program

* First obtain the subset of tickers by running the `ssm.ipynb` in the ss_module.
* After obtain a csv of recommend contracts by running the cfsm.ipynb in the cfs_module.

## Authors

* [Jonathan Riso](https://github.com/Jonathan-Riso)

## Version History

* 0.1
    * Initial Release

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments

* [Tony Riso](https://github.com/trisoheartrun) - Initial idea and contributions during initial release.