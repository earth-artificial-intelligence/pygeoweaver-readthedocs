# Getting Started

Welcome to the Pygeoweaver documentation! This guide will help you get started with using Pygeoweaver, a Python package that provides support for geoweaver functionalities.

## Table of Contents
- [Installation](#installation)
- [Quick Start](#quick-start)
- [Using Pygeoweaver](#using-pygeoweaver)
- [Additional Resources](#additional-resources)

## Installation

To begin using Pygeoweaver, you need to install it on your system. Pygeoweaver is available on the Python Package Index (PyPI), which means you can install it easily using `pip`.

```shell
pip install pygeoweaver
```

This command will install the latest version of Pygeoweaver and its dependencies on your machine. Make sure you have Python and `pip` installed and properly configured before running this command.

After pygeoweaver is installed, please run:

```shell
gw start
```

Finally, Open your browser and enter: http://localhost:8070/Geoweaver/. That is it.

## Quick Start

Once you have installed Pygeoweaver, you can quickly get started with the following steps:

1. Import the Pygeoweaver package in your Python script or interactive session:

```python
import pygeoweaver
```

2. Create a process using the `create_process` function. This function allows you to define the programming language, description, name, code, and other optional parameters for the process. Here's an example:

```python
process = pygeoweaver.create_process(
    lang="python",
    description="My first Pygeoweaver process",
    name="Process 1",
    code="""
        # Your process code here
    """
)
```

3. Explore the functionalities and methods provided by Pygeoweaver to work with processes, workflows, and other geoweaver-related tasks. Refer to the [API Reference](/en/latest/API%20Reference/create-process-from-file/) for detailed information on available classes and methods.

## Password Reset for Localhost

If you forget or need to reset the password for Geoweaver on localhost, run the following command in your terminal:

```shell
java -jar geoweaver.jar resetpassword
```

If you used `Docker`, use the following command:

```shell
docker run -t -i -v <YOUR_HOME_DIRECTORY>:/home/marsvegan/ -p 8070:8070 jensensun/geoweaver resetpassword
```

## Using Pygeoweaver

Pygeoweaver offers a comprehensive set of features for managing geoweaver processes and workflows. Here are some key aspects of working with Pygeoweaver:

- **Creating Processes**: Use the `create_process` function to define and create processes with the desired programming language, code, and other details.

- **Managing Workflows**: Pygeoweaver allows you to create and manage workflows by defining nodes and edges using the `create_workflow` function. You can specify the nodes and their dependencies to construct complex workflows.

- **Interacting with Geoweaver**: Pygeoweaver provides functions and methods to interact with a Geoweaver instance, enabling you to add processes, workflows, and perform other geoweaver-related tasks.

## Additional Resources

- **Report Issues**: If you encounter any issues or have suggestions for improvements, please report them on our GitHub repository [here](https://github.com/ESIPFed/pygeoweaver/issues).

Congratulations! You have completed the Getting Started guide for Pygeoweaver. You are now ready to dive deeper into Pygeoweaver's capabilities and build your own geoweaver processes and workflows. Happy coding!
