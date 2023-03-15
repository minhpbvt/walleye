# Step 1: Install Nginx and Gunicorn

To get started, you'll need to install Nginx and Gunicorn on your Linux server. You can do this by running the following commands:

```
sudo apt update
sudo apt install nginx python3-pip
sudo pip3 install gunicorn
```
These commands will update your package list, install Nginx and Python3 pip, and then use pip to install Gunicorn.
# Step 2: Clone the project repository

Once you have installed Nginx and Gunicorn, you can clone the project repository to your server using Git. If you haven't already installed Git, you can do so with the following command:
```
sudo apt install git
```
Next, navigate to the directory where you want to clone the repository and run the following command:
```
git clone https://github.com/minhpbvt/web-detecting-cracks-on-wall.git
```
# Step 3: Set up a Python virtual environment

Before installing the project dependencies, it's a good idea to set up a Python virtual environment to keep them isolated from other Python projects on your server. To do this, navigate to the project directory and run the following commands:
```
python3 -m venv env
source env/bin/activate
```
The first command creates a new virtual environment in a directory called `env` within the project directory. The second command activates the virtual environment, which changes your shell's Python interpreter to use the one installed in the virtual environment. Once the virtual environment is activated, you can install the project dependencies without affecting other Python projects on your server.
# Step 4: Install project dependencies

With the virtual environment activated, you can now install the project dependencies listed in the requirements.txt file. Run the following command from the project directory:
```
pip install -r requirements.txt
```
