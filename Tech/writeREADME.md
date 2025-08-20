# Writing a README file
I used to checkout the `Add a README file` checkbox whenever I create a new repo because I thought it was a useless file (It may have thought the same about my project). But now I understand its importance.

# Why README file
README file is the face of your repo. Haven't heard that judgmental proverb `Face is the index of the mind`.
People are not going to read each and every file to know what the project is about. The title 'final year project' never tells everything about your project (It needs an Asian kid's level IQ to get info just by the title). So it is crucial to write a good README file so that people can skip your project at first glance 😉.

# Basic MarkDowns
* ``#[SPACE]`` -> Heading (# h1, ## h2, ### h3)
* ``*[SPACE]`` -> makes bulletins
* ``**[TEXT]**`` -> Bold
* ``***[TEXT]***`` -> Italics
* ``>[TEXT]`` -> Blocked quotes like this
> This is a blocked quote
* ``[Title](LINK)`` -> To add hyperlinks
* ``![Title](URL)`` -> Add image or use img html tag as shown in [Cool stuffs](#cool-stuffs)
* \`\` -> for inline code

# Should contain
Here is a list of contents that should be present in a project repo
* Project Title
* Description
* Technology used (If any 💁🏻)
* How to use
* API Refs

## Optional
* Build Status
* Screenshots

## Cool stuffs
* **Shields** <img src="https://img.shields.io/badge/-cool-brightgreen">, yes something like this; You can find this in [shield.io](https://shields.io/badges) and use it using `<img>` tag
* Demo gif of your project working (videos won't work in git README)

```md
![Sierra Hotel India Echo Lima Delta SHIELD!](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExeW1vbzJuZzl2ZWE5NTN1YzFqazhyNjA2bGp4emhhc2J2cWJvM3g2biZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/1n59hHgrQgD3KN3fSu/giphy.gif)
```

![Sierra Hotel India Echo Lima Delta SHIELD!](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExeW1vbzJuZzl2ZWE5NTN1YzFqazhyNjA2bGp4emhhc2J2cWJvM3g2biZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/1n59hHgrQgD3KN3fSu/giphy.gif)

* While adding **code blocks**, you should consider using `js [enter][CODE]` like this. Because most markdown supports coding languages  and it will be easy to read for programmers. It adds text colors 👀
```js 
function uptown(){
    var day = "Saturday";
    console.log(day+" night and we in the spot");
}
```
* Using **HTML tags** - You can use some basic html tags to build elements like
```HTML
<h1 align="center">you know who I am</h1>
```
<h1 align="center">you know who I am</h1>
<br>

# Linking Contents
We can link that can guide to a specific part of the file. use `#` to select the heading of the content like this
```md
[Intro](#writing-a-readme-file)
```
* [Intro](#writing-a-readme-file)
* [Should contain](#should-contain)
* [Conclusion](#conclusion)

# Interesting Reads
* [Difference between markup and markdown language](https://medium.com/@sigireddyviswesh/difference-between-markup-and-markdown-language-e087bfff06d2)

# Conclusion
There are more, but I feel these are the most important ones or I'm not ready to spend more time on this. I forget where I read these things, but thanks to that person. And... yeah, that's it (this conclusion is just a formal thing no useful information here)