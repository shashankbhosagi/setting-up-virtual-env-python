# Setting up virtual enviroment in Python

#### Note: Make sure you have `virtualenv` installed in your PC
- To install
  ```bash
  pip install virtualenv
  ```


## 1)  Make a project directory first
```bash
mkdir project
cd project
```
![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/9a0e7c7c-b985-430c-b76f-b566b389b579)

## 2) Create virtual env using this command
```bash
python3 -m tool_name environment_name
```
- `tool_name` : it is the name of tool used to create virtual enviroment
- `enviroment_name` : name of environment ends up being the name of folder where everything is stored.

##### Note: generally the easiest tool used is `venv`

```bash
python3 -m venv venvTest
```
### Note: If you encounter such message, this will generally occur if you are creating virtual environment first time

![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/0410811f-c3b4-4205-95b8-30b6d715fc00)

- Solution is simple 
    - First check what version your python is 
    - Run following command
    ```bash
    sudo apt install python3.10-venv
    ```
    - The version should be according to your python version
    ![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/b15574e9-bd2c-48bf-be48-cbc5f8f81ee8)


#### After the virtual enviroment is created, create an file named app.py
![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/123802d2-5f58-44d4-b2b1-e9606842f1d0)


## 3) Activate the virtual environment
TO activate the virtual environment run this command
```bash
source venvTest/bin/activate
```
![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/261cee59-7332-4587-9fdb-ad3b6000e283)

<h3> Hurray 🎉 you have entered the virtual enviroment the name of the environment is shown before the username </h3>

#### Now as you have created virtual environment you can install all the dependencies for your app and run the python app

#### Note: When developing apps in python or any python framework makesure to maintain a `requirements.txt` inside the folder structure and keep adding name of libraries that you install during the development. And whenever I have to share with other person, he will directly activate the virtual environment and install all dependecies using `pip install -r requirements.txt`

## 4) Deactivating the virtual environment
```bash
source ~/.bashrc
```
![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/0cee2529-3986-4232-ad8d-2d89d06507a1)



## How to maintaina requirements.txt file

requirements.txt
```txt
flask==1.8.1
requests==1.0.1
```

- The above file `requirements.txt` shows how to store the name and version number.
- The version number is very important and if you don't mention it and say in future you install dependecies and run the project you may encounter many dependency issues, because as the version number change the new ways to use the library or dependecy are introduced so old methods will not work and your python application may not run!
- What is the significance of version number, it shown in below image.
  ![image](https://github.com/shashankbhosagi/setting-up-virtual-env-python/assets/78866224/4785bb51-4389-4f03-a2c5-5032a3f2ec0f)


Happy Coding and Enjoi 🎉




