<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>


## Setup 

------

#### Clone code-server
~~~
git clone https://github.com/daniel2mind/code-server;
~~~

------

#### Clone VS Code and install dependences
~~~
cd /path/to/code-server/lib && rm -rf vscode && git clone https://github.com/daniel2mind/vscode;

cd /path/to/code-server/lib/vscode && yarn install; 

yarn add bootstrap-node;
~~~

------

#### Compile VS Code
~~~
cd /path/to/code-server/lib/vscode && yarn compile; 
~~~

------

#### Install dependences in code-server path
~~~
cd /path/to/code-server && yarn install; 
~~~

------

#### Build code-server
~~~
cd /path/to/code-server && yarn build; 
~~~

------

#### Command to run code-server
##### (in /path/to/code-server)
~~~
node ./out/node/entry.js --port=8000 --auth=none
~~~