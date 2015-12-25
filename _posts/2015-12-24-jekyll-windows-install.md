---
layout: post
title: Run Jekyll on Windows
category : coding finder
tags : [coding, favorite, hobby]
---
**Run Jekyll on Windows**  

<http://jekyll-windows.juthilo.com/1-ruby-and-devkit>  

1. install Ruby(Ruby 2.2.3(x64) :  
Add Ruby executables to your PATH  
	<http://rubyinstaller.org/downloads/>  

    T

2. install Ruby DevKit(DevKit-mingw64-64-4.7.2-20130224-1432-sfx.exe) :  
	For use with Ruby 2.0 and above (x64 - 64bits only)  
	<http://rubyinstaller.org/downloads/>  

    go to Ruby DevKit Folder
    
    cd C:\RubyDevKit
    ruby dk.rb init
    ruby dk.rb install 

	if ruby dk.rb init has problem, add config.yml  
    - C:/Dev/Ruby22-x64  
	

3. install the Jekyll Gem  
	go to new forder for Jekyll Blog  
    > gem install jekyll  

4. install a Syntax Highlighter  
    > gem install rouge  
	Then, [_config.yml], set Rouge as syntax highlighter  
	highlighter: rouge  

5. install Python(version 2.7.11, Python 3 will not work)  
	Add Python.exe to Path > Entire feature will be installed on local hard drive  
	<https://www.python.org/downloads/>  

6. install pip  
	go to new folder for installing pip  
	download get-pip.py  
	<https://bootstrap.pypa.io/get-pip.py>  
	Then  
    
    > cd C:\pip  
    > python get-pip.py  
	or double click get-pip.py  
    

7. install the Jekyll Gem  
    > gem install wdm  


**Sub-Directories**
If pages are defined in sub-directories, the path to the page will be reflected in the url.
Example


    .
    |-- people
        |-- bob
            |-- essay.html






Github  
//	> git clone https://github.com/ID/ID.github.com	//github files > Desktop  
//	> cd ID.github.com  
> jekyll --serve	//start <http://localhost:4000>  
	> git init		  
	> git remote add master https://github.com/timibird/timibird.github.com.git  
	>git add *  
	>git commit -a -m "test commnet"  
	> git push master master --force  
  
  
JDK 설치  
EditPlus 설치(JAVA 환경 셋팅)
GitHub Desktop 설치
