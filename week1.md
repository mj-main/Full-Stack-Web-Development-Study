## 1주차 내용
1. 풀스택 웹개발이란
2. 개발환경 세팅(git, npm)
3. Bootstrap


### 1. What is Full-Stack Web Development?
- 프론트엔드는 콘텐츠를 사용자에게 렌더링하는 곳이며, 백엔드에 의해 지원된다.
- 풀스택 웹 개발은 3가지로 구성된다.
    - 프레젠테이션: 사용자에게 콘텐츠를 제공하는 UI
    - 비즈니스 로직: 데이터 검증 및 동적 콘텐츠 처리
    - 데이터 액세스: 데이터 저장 및 API를 통한 접근 



### 2-1. Setting up Git

```
# Download git
https://git-scm.com/downloads

# Check the version
$ git --version

# Configure username
$ git config --global user.name "Your Name"

# Configure email
$ git config --global user.email <your email address>

# Check configuration
$ git config --list
```

### 2-2. Basic Git Commands
```
# Initialization
$ git init

# Check status
$ git status

# Add files to stage
$ git add .

# Commit stage
$ git commit -m "first commit"

# Check the log
$ git log --oneline

# Check out earlier commit
$ git checkout <second commit's number> <filename>

# Reset
$ git reset HEAD <filename>

# Set remote origin
$ git remote add origin <repository URL>

# Push commit
$ git push -u origin master

# Clone repository
$ git clone <repository URL>
```

### 2-3. Setting up npm
```
# Download npm
https://nodejs.org

# Initialization
$ npm init

# Install npm modules, lite-server
$ npm install lite-server --save-dev

# Edit package.json
{
  "name": "week1",
  "version": "1.0.0",
  "description": "This is the Git and Node basic learning project",
  "main": "index.html",
  "scripts": { 
    "start": "npm run lite", # add code
    "test": "echo \"Error: no test specified\" && exit 1",
    "lite": "lite-server" # add code
  },
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "lite-server": "^2.6.1"
  }
}

# Start server
$ npm start

# Add gitignore
$ node_modules
```


### 3-1. Why Front-end Web UI Frameworks?
- Resposive web design
- Cross-browsing
- Increase productivity
- Community support

### 3-2. Introduction to Bootstrap

![dd](https://www.ostraining.com/cdn/images/blog/bootstrap-popularity/wappalyzer-frameworks.png)
[Market share](https://www.ostraining.com/blog/webdesign/bootstrap-popular/)

- Most popular HTML, CSS, and JavaScript based framework
- Designed for developing responsive mobile first websites

### 3-3. Getting started with  Bootstrap
[Bootstrap4-starter.zip](https://d3c33hcgiwev3.cloudfront.net/bOGnMCzEEeiTdA5yoE99Fg_6da6f2f02cc411e8b484f7e801bd0278_Bootstrap4-starter.zip?Expires=1616544000&Signature=E3u0Qa9Za0k5QwEwkTrSwbdK8A6mN4DqEjLU7MJGJiM3WzQ5DZSBhTNkXHzPUelbKjVokoffGTrVEeYc5KhkaQJ4xUzUCZVE4rXihvj7bfi4HJG~CWvftdlApjeRHBdAmeUldPl5D6it8szMpE~W3KI4VpwM~3Ol-ktPSpmg1mI_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
```
# Download and unzip file
Bootstrap4-starter.zip

# Install node modules
$ cd  conFusion 
$ npm install 


# Download bootstrap
$ npm install bootstrap@4.0.0 --save
$ npm install jquery@3.3.1 popper.js@1.12.9 --save
```

Insert follow code to html file
```
# In the <head> tag before <title>
<!-- Required meta tags always come first -->
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<meta http-equiv="x-ua-compatible" content="ie=edge">
<!-- Bootstrap CSS -->
<link rel="stylesheet" href="node_modules/bootstrap/dist/css/bootstrap.min.css">

# just before the end of the <body> tag
<script src="node_modules/jquery/dist/jquery.slim.min.js"></script>
<script src="node_modules/popper.js/dist/umd/popper.min.js"></script>
<script src="node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
```


### 3-4. Responsive Design
- Render websites consistently on devices of different screen sizes
- Foundations: Grid system, Fluid image, Media queires

### 3-5. Bootstrap grid system
```
# viewport meta tag: Set screen width to the device width
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

# container class
<div class="container"> ...

# Dividing the content into rows
<div class="row"> ...

# Applying column classes within each row
<div class="col-12 col-sm-4 col-md-3"> ... </div>
<div class="col col-sm col-md"> ... </div>

# Align center: vertical  
<div class="row row-content align-items-center">

# Align center: horizontal
<div class="row justify-content-center">             
    <div class="col-auto">

```