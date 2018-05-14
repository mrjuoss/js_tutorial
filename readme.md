# The Learn Enough Society
## Hello Word
### 1.1. JS in a web browser
Ikuti langkah-langkah dibawah ini
1. mkdir -p ~/Code/js_tutorial
2. cd ~/Code/js_tutorial
3. touch index.html
4. touch index.md
5. atom .
6. git init
7. git add -A
8. git commit -m "Initialize Repository"
9. Edit file index.html
10. git commit -am "Add a Javascript alert"
11. Create a new Remote Repository at Github
12. git remote add origin https://github.com/<username>/js_tutorial
13. git push -u origin master
14. Visit your site at https://<username>.github.io/js_tutorial

### 1.2. JS in a REPL (Read, Eval, Print, Loop)
REPL is a Programm that __READ__ s input, __EVAL__ uates it, __PRINT__ the results (if any) and then __LOOP__ s back to the read step.

#### REPL from BROWSER CONSOLE

__BROWSER CONSOLE__ is valuable debugging tool, as it has access to the full DOM and other aspect of our application's environment, as well as displaying any warning or errors that might affect our application.

In Javascript we use console.log (log is function in javascript) Ex. console.log ("Hello Word");

#### REPL from NODE PROMPT
Ikuti langkah di bawah ini:
1. $ which node (enter)
2. If node isn't present on your system, you should install it at your system
3. $ brew install node
4. node (enter)
5. console.log("Hello Node");
6. in console node, alert is not defined (ReferenceError: alert is not defined)

### 1.3. JS in FILE
Ikuti langkah di bawah ini:
1. touch hello.js
2. edit hello.js with your text editor
3. link file hello.js to file index.html
4. reload the web browser
5. if running in NODE Prompt, ketikkan node <nama_file.js> Ex. node hello.js

### 1.4. JS in a SHELL SCRIPT
Ikuti langkah di bawah ini:
1. touch hello (without extention file)
2. $ which node (hasilnya berupa lokasi node terinstall)
3. Copy lokasi file output langkah nomor 2 diatas
4. edit file hello
5. make file hello executable using chmod ($ chmod +x hello)
6. execute with this command ./<nama_file> Ex ./hello
7. Jika ingin melakukan eksekusi dengan nama file langsung maka lakukan setting sebagai berikut
  * $ atom ~/.bash_profile
  * export PATH file (Contoh sebagai berikut)
    * alias lr='ls -hartl'
    * export PATH="~/Code/js_tutorial:$PATH"
  * $ source ~/.bash_profile

## STRING

Javascript support common special characters such as __tabs__ (\t) and __newlines__ (\n). Contoh console.log("Selamat \t Datang \n Para Tamu");

### 2.1. Concatenation and Interpolation

__Concatenation__ is Joining String together. __Interpolation__ is Putting variable content into Strings.

__Concatenation__ Example :

```Javascript
1. $ node
2. > "Foo" + " bar"; // String Concatenation
3. Output : Foo bar
```
__Interpolation__ Example:

```Javascript
1. let firstName = "Arif";
2. let lastName = "Mujaki"
3. let fullName = `My Fullname is ${firstName} ${lastName}`;
4. Output : My Fullname is Arif Mujaki
```

### Properties, Booleans and Control Flow

Almost everything in Javascript, including strings, is an __OBJECT__

Example :

```Javascript
1. $ node
2. > "mujaki".length // Accessing the "length" property of a strings
3. Outputnya 6 (mujaki terdiri dari 6 string)
```

```Javascript
1. > "mujaki".length > 3
2. Outputnya TRUE
3. > "arif".length > 7
4. Outputnya FALSE
```

```Javascript
1. > let password = "foo";
2. if (password.length < 6) {
    "Password is to short"
   }
3. Outputnya Password is to short
```

### METHODS
