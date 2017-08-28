## babel
#### 安装babel-cli
     npm install babel-cli --save-dev
#### 举例
    babel [srcfile.js] --out-file script-compiled.js//将js文件翻译
    babel src --out-dir lib //将src文件夹下的文件翻译成lib下的文件
    babel --watch src --out-dir lib
#### 在package.json里添加脚本
     "scripts":{
       "test":"echo\"Error: no test specified\" && exit 1",
       "build": "babel src --watch --out-dir lib"
     },
     npm run build

     npm install babel-preset-es2015 --save-dev//安装es2015相关的插件
     在项目的根目录下创建babel.rc文件
     {
		"presets":["es2015"]
     }
#### 安装babel-preset-react
     npm install babel-preset-react --save-dev
     在项目的根目录下创建babel.rc文件
     {
		"presets":["es2015", "react"]
     }
#### 安装gulp， gulp-babel
     npm install gulp gulp-babel --save-dev
     创建gulpfile.js
