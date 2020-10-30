# MemorizeIT

Project is created to **increase memory and focus** among children or adults who would like to take part in training. 
Rules of game are quite simple. You just need to count elements displayed on screen and remember their type. At the end 
you will be asked to write down your results and confront them with exact ones. This will be verified by marking your 
answer with proper color (correct - green, not - red). Difficulty of game can be increased by adding more types of 
elements to count, mixing their colors, turning sound off or changing time dedicated to each wave. It is also more 
difficult to play normal game mode (instead of static), because figures are moving which is additional distraction. *I 
wish you enjoyable experience with game and best results in memory training. Good luck!*

![Menu](https://raw.githubusercontent.com/ethru/memorizeit/master/img/menu.png)

## Installation

```
$ git clone https://github.com/ethru/memorizeit.git
$ pip install memorizeit/.
```
**Beware:** Application was developed and tested on **Fedora**. Some functions may not work or behave in different way 
on other systems.

## Run

Open terminal and type: `$ memorizeit` or `$ python -m memorizeit`

## How to configure game:
- settings are stored in game directory - *settings.json* file
	![Config file](https://raw.githubusercontent.com/ethru/memorizeit/master/img/config.png)
	- making changes in application settings menu updates this file
	- removing it will restore default game settings
- default images (displayed in static mode) are stored in game directory - *img/elements/*
	- they can be removed (figures will be displayed instead)
	- or replaced (application scales images automatically - user do not need to worry about it)
	![Static gameplay](https://raw.githubusercontent.com/ethru/memorizeit/master/img/static.gif)
- sound of new elements appearing in game is stored in application directory - *sound.ogg*
	- it can be replaced by any sound in ogg format (just make sure it won't be too long to avoid unpleasant experience)
- game can be configured in applications settings menu, it contains options like:
![Settings menu](https://raw.githubusercontent.com/ethru/memorizeit/master/img/settings.gif)
	- figures - number of unique types of the elements which may appear during game
	- time - duration of game in seconds
	- speed - level of speed difficulty from slowest to fastest
	- colors - level of color difficulty (not used with images in static mode)
		- Easy - each type of elements displayed in same color
		![Easy mode](https://raw.githubusercontent.com/ethru/memorizeit/master/img/easy.gif)
		- Medium - each wave of elements displayed in various color
		![Medium mode](https://raw.githubusercontent.com/ethru/memorizeit/master/img/medium.gif)
		- Hard - every element displayed in various color
		![Hard mode](https://raw.githubusercontent.com/ethru/memorizeit/master/img/hard.gif)
	- sound - specifies if sound should be used with every new wave of elements
- **spoiler alert**: for hidden game mod take a look at `class Figure3D` and `class Wave3D` in *figure.py* module

## How to play game:
- adjust game settings
- pick mode: normal (new) or static game
- count elements of each type separately
- write down and submit your result
- compare it with exact values
- change game difficulty and make progress
![Summary](https://raw.githubusercontent.com/ethru/memorizeit/master/img/result.gif)

## Project Information

##### Documentation

Generated by [pdoc3](https://pdoc3.github.io/pdoc/) and included in 
[docs](https://github.com/ethru/memorizeit/tree/master/docs) directory. Open it 
[here](https://ethru.github.io/memorizeit/).

##### Requirements

- Python3.7+
- Check [requirements.txt](https://raw.githubusercontent.com/ethru/memorizeit/master/requirements.txt) file to see used 
modules and their version.

##### Author

Adrian Niec

##### License

This project is under the MIT [License](https://raw.githubusercontent.com/ethru/bookmeister/master/LICENSE)
