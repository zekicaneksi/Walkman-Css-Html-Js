# Walkman-Css-Html-Js
Using the Web Audio API, i created a Walkman music player. The code most likely doesn't use the best practices and instead bad practices, also the code isn't elegant. But it works and doesn't cause any bugs (so far, it didn't anyways).

![image](https://user-images.githubusercontent.com/59491631/173868928-045d375d-aae5-4fc0-9cd5-eab3d3901710.png)

### For live demo;
https://htmlpreview.github.io/?https://github.com/zekicaneksi/Walkman-Css-Html-Js/blob/main/walkman.html

### How to Implement

You can just copy paste the code and use it. All you need to do is;
- change the stylesheet link href attribute.
```
        <link rel="stylesheet" href="https://raw.githubusercontent.com/zekicaneksi/Walkman-Css-Html-Js/main/walkman.css">
```
- change the setUp() function which arranges the audio urls and dynamically adds option tags to the select tag. also, sets the size of the select element;<br></br> (And also, obviously call this function sometime to intialize the walkman.)
```
        function setUp(){
            audioUrl=[
                'https://raw.githubusercontent.com/zekicaneksi/Walkman-Css-Html-Js/main/winning-elevation-111355.mp3',
                'https://raw.githubusercontent.com/zekicaneksi/Walkman-Css-Html-Js/main/loneliness-of-the-winner-110416.mp3',
                'https://raw.githubusercontent.com/zekicaneksi/Walkman-Css-Html-Js/main/forest-lullaby-110624.mp3',
                'https://raw.githubusercontent.com/zekicaneksi/Walkman-Css-Html-Js/main/anthem-of-victory-111206.mp3'
            ];
            let select = document.getElementById('SongsSelect');
            select.options.add(new Option('Winning Elevation', 'Winning Elevation'));
            select.options.add(new Option('Loneliness of the Winner', 'Loneliness of the Winner'));
            select.options.add(new Option('Forest Lullaby', 'Forest Lullaby'));
            select.options.add(new Option('Anthem of Victory', 'Anthem of Victory'));
            select.setAttribute('size','4');

        }
```
- and lastly, change the walkman's positioning values in the stylesheet.

The code doesn't have many lines, and i tried to name everything properly.
So, you can just edit the javascript code and html a little bit, and change the css entirely to make it look better (that is if you think you can...).
