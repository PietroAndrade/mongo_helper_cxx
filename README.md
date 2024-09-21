# mongo_helper_cxx

## Build options for linux


1. Install pip
```sh
    sudo apt install python3-pip -y
```

2. Create a python env
```sh
python3 -m pip install --user virtualenv
python3 -m venv venv
```

3. Activate env
```sh
source venv/bin/activate
```

4. Install conan
```sh
sudo pip install conan
```

5. Detect conan profile
```sh
conan profile detect
```

6. Use `conan` as the build tool and also install the dependencies using:
```sh
conan install . --build=missing --profile=build.conanprof
```