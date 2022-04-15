## How to install virtual environment: 

To install and activate virtual environment, follow these steps. They can differ based on your operating system.

### 1. As a first step, go to your PyLadies course folder you will be working this semester (in command line)
eg. cd pyladies_data_course

### 2. Install virtualenv
This step is a bit different for windows and Unix/MacOS:

Windows: py or python3 could be a difference based on your version

```shell 
py -m pip install --user virtualenv
``` 
OR 
```shell
python3 -m pip install --user virtualenv
```

Unix/MacOS: 

```shell 
python3 -m pip install --user virtualenv
```

### 3. Create virtual environment
"Second" venv in this command is a name of your environment. You can change that, but use your chosen name in all other commands.

Linux: ```python3 -m venv venv``` OR older versions  :   ``` virtualenv -p python3 venv```

Windows: ```py -3 -m venv venv```

MacOS: ```python3 -m venv venv```

### 4. activate virtual enrvironment
Here be careful with direction of slashes in the path.

Windows: ```venv\Scripts\activate```

Unix/MacOS: ```source venv/bin/activate```


After this command you should see (venv) infront of command line prompt. This means you are succesfully inside your virtual environment. Everytime you want to start your environment again, run this command from your course folder.

## leave environment

All systems: ```deactivate```
