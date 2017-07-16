# [Duck]() ![logo][logo-xs]

## Note to readers

This README isn't complete yet as duck is still in early development phase. Please note that duck is still useable.

We apologize for the lack of informations on this readme.

## Installation

### Dependencies

Duck requires curl and go to be installed. To install go please follow [this link](https://golang.org/doc/install). Curl can be easily installed with most package manager like :

`sudo apt-get install curl`

or

`brew install curl`

### Duck

Duck installation is easy :

```
curl https://raw.githubusercontent.com/snwfdhmp/duck/master/INSTALL.sh | bash
```

## Usage

`duck <action> [args]`


## Getting started

Create a new directory for your projects

```
$ mkdir my-project
$ cd my-project
```
Init a duck repo in this directory

```
$ duck init
Name: tictactoe
Lang: go
Main: game.go
```

Install the ducklings you want (see a list of ducklings [here](#))

```
$ duck install snwfdhmp/std
$ duck install snwfdhmp/go
$ duck install snwfdhmp/cpp
$ duck install snwfdhmp/junk
```

## Make a duckling

Ducklings are duck's most interesting part.
They are highly hackable jobs you configure to fit your development environment perfectly.

We provide some ducklings examples in <code>.duckling/</code>

<code>.duckling/go.duckling</code>

```json
{
	"Ducklings":[
		{
			"Label":"compile",
			"Description":"compile project",
			"Commands":["go build -o $name $main"],
			"Aliases":["build"]
		},
		{
			"Label":"create",
			"Description":"create necessary files for a new package",
			"Commands":[
				"mkdir $1",
				"touch $1/$1.go"
				]
		}
	]
}
```


## Contributing

Duck is open to contributors, feel free to open issues as well.

## Author

- [snwfdhmp](http://github.com/snwfdhmp) (I'm currently the only one on this project.)



[logo-xs]: https://www.github.com/snwfdhmp/duck/raw/master/ressources/img/logo-xs.png "Logo"