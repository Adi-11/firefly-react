# firefly-react
A React Component for showing interactive animation of fireflies on canvas . As seen on the main page of http://thomso.in



## Some Highlights : 
* ### No external dependecies required ( yeaa ! pure vanilla )
* ### library size is only 16kb ,  cz Size Matters xxd
* ### Project Uses
     * TypeScript
     * Rollup 

## USAGE : 

```js
npm i firefly-react
```

Import it into your React Project 
````js
import Firefly from "firefly-react"
````
You can add an Array of colors and the fireflies thus generated will get its color from this array in  a random fashion  :

```js
const colors =  ["Blue ", "Green", "Red", "Orange"];
```

```JSX
   <Firefly numberOfBirths={2} canvasWidth={window.innerWidth} canvasHeight={window.innerHeight} colors={colors} changeDirectionFrequency={10} randomMotion={true}></Firefly>
```

## The Result

https://user-images.githubusercontent.com/43696525/115184714-0b7ee380-a0fc-11eb-8b6e-1718431532ed.mp4



## Props :

Props | Value | default |  description 
------------ | ------------- | ----------- | ------------
numberOfBirths  | [ 1 - 10 ] | 2 |   this contolls the number of fireflies that will born when the mouse will be moved 
canvasWidth | [0,SAFE-INT] | HMTL CANVAS DEFAULT |   sets width of the canvas 
canvasHeight | [0-SAFE_INT] | HMTL CANVAS DEFAULT |  sets the height of the canvas
colors   | [ ] | ["black"]|  fireflies thus generated will be randomly alloted the colors from this array 
randomMotion| bool | false  |   this is the most significant and amazing feature that mimics the random motion of a read world firefly while flying,set to `true` and see the magic 
changeDirectionFrequency | [10-120] degree Angle | 30 | this value controlls how often the firefly will change the direction in random walk motion, this do not do anything alone if randomMotion props is set to false.


## Want to Contribute ?
Contributing to Open source is self rewarding and i love being part of it , if you too are excited about it , i would love to collaborate :3 .
Currently we need help with :
1.Using multithreading concepts to boost our  canvas rendering
2.particle pooling and hence performance optimization
3.I do believe this project has immense potential to offer some good out there , so any proposal for  new feature addition would be highly appreciated .
4.Strong type checking and dynamic object validation would also make this library robust 

