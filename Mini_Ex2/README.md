# Mini_Ex2:
**Objective:**
To comprehend the the notion of fun through eksperimenting
with computational drawing possibilities, and Goriunova's text concerning the notion of fun.

### FUN.js
This might sound weird but i found that this mini_ex2 was actually quite hard to do, 
compared with my previous mini_ex1. I think that one of the reasons why is that I have been sick, 
and i have therefore strugled with finding my inner humoristic programmer. I have during the past week had the sensation of having a head filled with this slippery aqueous secretion substanse called mucus. my nose has become a highway for this substance to exit my internal system. This has led to my nose feeling sort of disemboidiet with the rest of my face. 
</br>
</br>
![alt text](https://github.com/Pacour/Aesthetic_Programming_2018/blob/master/Mini_Ex2/Screen%20Shot%202018-02-18%20at%2023.39.53.png "Logo Title Text 1")
</br>
Press the [RawGit](https://cdn.rawgit.com/Pacour/Aesthetic_Programming_2018/9af8329a/Mini_Ex2/Source/index.html) to run my code.
</br>
</br>
In my struggle to be fun and creative, I then started out with looking at the word "fun", and I tried to perceive the word fun as an abriviation for something else. So FUN stands for Fundamentally Uncontrollable Nose, which sort of tells my story of being sick and needing to constantly blow my nose. When i finally had figured out what my story was I then developed this image in my mind of how i wanted it to look. So my idea was to see this head from the side and then having the nose just be a very simple triangle and then perhaps using the ```random()``` to make the nose jitter along the X-axis. I also thought that having the angle from the side, rather than a more front-face angle would help put more emphasis on the uncontrollable grownth of the nose. A very crucial part of the assignment was to only use simple 2d shapes and try to use ones imagination to get an idea that could be expressed as closely to the idea as possible with the limited knowledge and tools that we currently posses. So this mini_ex also somewhat build on the minimalistic concept of less is more. I wanted only to add as many basic shapes as I needed in order to communicate my story. since one of the things I learned from my last mini_ex was how to load in a .mp3 I used that knowledge to load in a sample of someone sneezing, which I did to further ensure that my story is comprehendsible.

**The Code:**
```javascript
/* This is Mini_Ex2, where I explore FUN in programming
using only simple shapes and functions from the p5 library
*/
var s = 'F-undamentally U-ncontrollable N-ose';
var song;

function setup() {
  createCanvas(600, 600);
  song = loadSound('BeezSneez.mp3', loaded);
}

function loaded(){
  song.play();
  song.setVolume(0.4);
}

function draw() {
  background('#f0f0f');
  frameRate(10);
  strokeWeight(2);
  stroke(0);
    fill(50);
      text(s, 10, 10, 70, 80);
    fill('rgb(255, 206, 206)');  // The Head
      ellipse(width/1,width/2, 300,350);
    fill(0);
      ellipse(width/1.2,width/2.4, 10,15);
      ellipse(width/1.2,width/1.5, 50,40);
    fill('rgb(255, 206, 220)');  // The Nose
      triangle(width/1.3, width/2, random(0,450), width/2.3, width/1.3, width/2.5);
    fill(222); //Handkerchief
      quad(449, 305, 317, 344, 380, 413, 469, 304);
        quad(470, 305, 317, 320, 380, 413, 430, 304);
    stroke('green'); //Mucus
    strokeWeight(10);
      line(469, 302, 468, random(302,368));
}

function mousePressed(){
  console.log(mouseX, mouseY); //utility for finding X,Y Coordinates
}
```
### What is fun in the context of programming?
As Goriunova points out in her text, the word Fun is a problematic one, since it can either mean; the creative enjoyment of exploiting something very complex, it could be this stupefaction one gets through consumption or it could just be out right avioded and instead take a more conceptual or maybe even more disturbing approach, and lead to some more inventive modes of thinking. I think in my case that exploring fun through this more conceptual mathematical approach I was able to conjour up something thats not necessarialy super funny, but maybe construct this actually quite bizar situation. A situation that could not have been illustrated had I not had the unconstrained purposelessness space it needed, and my curious mind towards the code. I am still quite puzzled in relation to how wit could ever be a skill which could be used to learn, teach or evaluate hacking? Goriunova does however make a connection to Freuds economic thinking as judgement, in which she puts forth that "the most succesful joke relies on scarce means to achive the richest outcome" (Goriunova, 2014, p. 3). perhaps could my FUN.js be said to might have some scarcity in relation to have ruffly it is programmed, and that this scarcity is actually what might make it funny or witty in a sense. I am not exactly certain that I find it truly funny, I do however find that it's telling a story about a situation of sorts, one of scarcity of motivation to make something really complicated. 

- (Goriunova's text: Goriunova, Olga. Fun and Software: Exploring Pleasure, Paradox and Pain in Computing. Bloomsbury Academic, 2014, pp.1-19)
