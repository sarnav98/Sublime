# Sublime


MAC OS Install - 

1. /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

2. brew install gcc

3. cd /usr/local/bin/

4. ln -s g++-10 g++

5. ls

6. clear

7. LOGOUT

-------------------------------

G++ Build - (SUBLIME)

{
  "cmd" : ["g++ $file_name -o $file_base_name && gtimeout 4s ./$file_base_name<inputf.in>outputf.in"], 
  "selector" : "source.c",
  "shell": true,
  "working_dir" : "$file_path"
}

--------------------------------------
Making bits/stdc++.h work - 

simply put (stdc++.h) into /Applications/Xcode.app/Contents/Developer/Platforms/ChosenTargetPlatform/Developer/SDKs/ChosenMacOSSDK/usr/include/bits

MAKE SURE TO MAKE A FOLDER named - bits

----------------------------------------

Sublime Window setup - COMMAND + OPTION + 3

----------------------------------------

Create two files - inputf.in   &&  outputf.in 

----------------------------------------

=========================================================

Windows Setup ->

Sublime Build - 

{
    "shell_cmd": "g++ \"${file}\" -std=c++1y -o \"${file_path}/${file_base_name}\"",
    "file_regex": "^(..[^:]*):([0-9]+):?([0-9]+)?:? (.*)$",
    "working_dir": "${file_path}",
    "selector": "source.c, source.c++",

    "variants":
    [
        {
            "name": "Run",
            "shell_cmd": "g++ \"${file}\" -std=c++1y -o \"${file_path}/${file_base_name}\" && \"${file_path}/${file_base_name}\""
        }
    ]
}

---------------------------------------------

Download and Install MINGGW and Add it to ENVIRONMENT PATH

---------------------------------------------

