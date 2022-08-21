# Burpsuite-Pro
Crack burp suite pro in Macbook M1/M2

1. open terminal and check the java version, java version must be higher than 11. Type command: **java --version**
https://download.oracle.com/java/18/latest/jdk-18_macos-aarch64_bin.dmg

2. After java is complete we have to download Burpsuite Profesional latest version .jar & download bootloader.jar
https://portswigger.net/burp/releases/professional-community-2022-8-2?requestededition=professional&requestedplatform=jar
https://drive.google.com/file/d/156hh9GhVOWhefr2hzya0hPdekn4F6AkC/view?usp=sharing

3. Now copy both the .jar files and paste a new folder > open terminal in this new folder. Type command : **java -jar burploader.jar**

![CleanShot 2022-08-21 at 07 31 48](https://user-images.githubusercontent.com/26188697/185770488-3c1af956-f063-4d8b-82d7-102985872f0f.png)

 4. After this click on the RUN button in the popup and paste the license key.
 
 5. When you have to launch burp suite pro again, open terminal in this new folder and type command : 
 **<p>java -noverify -javaagent:burploader.jar -jar burpsuite_pro_v2022.8.2.jar</p>**
 
 *Tips: make aliases if you using zshrc*
 
 1. open ~/.zshrc
 **<p>alias burp='java -noverify -javaagent:/Users/yourdir/Documents/burp/burploader.jar -jar /Users/yourdir/Documents/burp/burpsuite_pro_v2022.8.2.jar'</p>**
 2. source ~/.zshrc
 3. type command: **burp**
 
 ![CleanShot 2022-08-21 at 07 41 52](https://user-images.githubusercontent.com/26188697/185770747-9b1da209-1db3-4627-871e-43dd25668bb1.gif)
