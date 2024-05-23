# Grammar-Checker
codecademy//js//beginners//practice
let story = 'Last weekend, I took literally the most beautifull bike ride of my life. The route is called "The 9W to Nyack" and it stretches all the way from Riverside Park in Manhattan to South Nyack, New Jersey. It\'s really an adventure from beginning to end! It is a 48 mile loop and it literally took me an entire day. I stopped at Riverbank State Park to take some artsy photos. It was a short stop, though, because I had a freaking long way to go. After a quick photo op at the very popular Little Red Lighthouse I began my trek across the George Washington Bridge into New Jersey. The GW is a breathtaking 4,760 feet long! I was already very tired by the time I got to the other side. An hour later, I reached Greenbrook Nature Sanctuary, an extremely beautifull park along the coast of the Hudson. Something that was very surprising to me was that near the end of the route you literally cross back into New York! At this point, you are very close to the end.';

let storyWords = story.split(' ');
let unnecessaryWord = 'literally';
let misspelledWord = 'beautifull';
let badWord = 'freaking';

console.log(storyWords.indexOf('Last'));

let count = -1;
storyWords.forEach(word => {
count++;
});

console.log(storyWords[0])

console.log(count)

storyWords = storyWords.filter(word => {
  if(word !== unnecessaryWord) {
    return word;
  }
});

 storyWords.map((word) => {
if (word == misspelledWord){
 storyWords[6] = 'beautiful';
  return storyWords;
}
});

badWordIndex = storyWords.findIndex((word) =>{
if (word == badWord){
return storyWords.indexOf(badWord);
}
});

console.log(badWordIndex+badWord)
storyWords[78] = 'really';

let lengthCheck = storyWords.every((word) =>{
if (word <= 10){
return word
} 
});

console.log(lengthCheck)


const result = storyWords.forEach((word) => word.length > 10);
// filter will also do the same
console.log(result)



storyWords[111] = 'jaw dropping';

//console.log(x);
console.log(storyWords.join(' '));

