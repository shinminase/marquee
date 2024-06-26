# marquee
a github svg that displays blinkies and pixels

<div align= center>
      sample:
</div>
<img src="sample.svg"></img>
<hr>


<details>
<summary> 
<h2>setting up the repository</h2>
</summary> 
1. assuming you already have a readme setup on your profile, you may create a folder under your github readme. 
<br> to make things all tidy i'll name it under user/images/svg<br><br>

![](https://files.catbox.moe/cy7l5h.gif)
<br><br>
2. copy and paste the code from [blankcode](https://github.com/shinminase/marquee/blob/main/blankcode.svg) here into the repository screen, then finally add "marquee.svg" at the end<br><br>
![](https://files.catbox.moe/ucmoz9.gif)
<br><br>
3. <b>HIT THAT COMMIT CHANGES BUTTON!</b>
<br><br>
4. now you should have something like this in ur folders.
![](https://files.catbox.moe/irv8rv.png)

</details>
<hr>
<details><summary><h2>working out the svg</h2></summary> 
1. if you go into the code, press the edit file button for marquee.svg
<br> you should be greeted with something a little like this. here's a breakdown of all the things

![](https://files.catbox.moe/vyyiua.png)
<br><br>

2. my default width and height listed in the blankcode are 150x20 for blinkies. however, you can change this as you wish.
<br> to put ur images, convert them to base64 first. use [base64-image.de](https://www.base64-image.de/)

![image](https://github.com/shinminase/marquee/assets/139236438/a5939516-c83e-4f42-aa7a-c5342a1d9859)
<br>
3. replace "base64 here" in the code with the actual base64 code of the image.
```
<g transform="scale(1.5)">
      <image xlink:href="base64 here" width="150" height="20" x="320" y="25" />
    </g>
```
sample:
```
<g transform="scale(1.5)">
      <image xlink:href="data:image/gif;base64,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" width="150" height="20" x="0" y="25" />
    </g>
```
unfortunately the code is very long since its base64. github doesnt allow normal image links on svgs
<br><br>
4. repeat this process BUT make sure u change the x property so that it doesnt overlap with eachother! btw if u want to make it so that the images refresh faster, change the following code snippet:
```
100% {
        transform: translateX(-250%);
      }
```
if you only plan on having three blinkies , i recommend changing it to -100%
</details>
<hr>
<details>
<summary> 
<h2>putting it on your github readme</h2>
</summary> 
  
This one's like really self explanatory. feel free to remove the a href tags, i only put it there so more people can access the tutorial

```
<a href="https://github.com/shinminase/marquee/">
  <img src="images/svg/marquee.svg"></img>
</a>
```

if u use markdown
```
![marquee](images/svg/marquee.svg)
```

<hr> 
</details>
<h1> happy coding! <img src="https://files.catbox.moe/n1pa93.gif"> - serph </h4> 

