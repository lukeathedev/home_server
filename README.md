# Home Server

Home Server is a project that allows users to set up a local network server that acts like a micro social media, where users can follow, message and share files with each other.

## Getting Started

If you've ever accessed the command line, you'll find this pretty trivial. We'll go through installing and setting-up all of the necessary components to get the server up and running.

### Prerequisites

In order to host *Home Server*, you'll need to install [Python 3](https://www.python.org/about/gettingstarted/). All of the other tools will be installed through *Python* and its package installer, *pip*.

### Installing

Getting Home Server to start isn't all that hard. As long as you follow the commands, you'll get it running in no time! Clone the repository and extract it to a desired location. Then, fire up the command line on the *home_server* directory.

Follow the steps below on your command line to set-up the environment.

#### For Windows

\#1: Setting up the environment

```
py -m venv env
```

\#2: Activating the environment:

```
.\env\Scripts\activate
```

\#3: Installing the required packages:

```
pip install -r requirements.txt
```

\#4: Generating the *home_server* database:

```
flask db upgrade
```

\#5: Running the server:

```
flask run
```

#### For macOS and Linux

\#1: Setting up the environment

```
python3 -m venv env
```

\#2: Activating the environment:

```
source env/bin/activate
```

\#3: Installing the required packages:

```
pip install -r requirements.txt
```

\#4: Generating the *home_server* database:

```
flask db upgrade
```

\#5: Running the server:

```
flask run --host=0.0.0.0
```

With the server set-up and visible in your home network, navigate to *localhost:5000* on your web browser. From there, you should be able to register, login and user the **Home Server** app.


## Deployment

Not currently deployable.

## Built With

* [Flask](http://flask.pocoo.org/) - Back-end Python based microframework
* [Bootstrap](https://getbootstrap.com/) - Front-end HTML toolkit
* [VSCode](https://code.visualstudio.com/) - Open source code editor

## Contributing

More information will be provided soon.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Luke A (lukeathedev)** - *Initial work*.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* **Miguel Grinberg** for providing a fantastic [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
* The [Stack Overflow Community](https://stackoverflow.com/) for providing great information on recurring development issues
