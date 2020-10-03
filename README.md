# changeBackgroundColor.js
This is a JavaScript program that changes the color of the background when a button is pressed

const colorBtn = document.querySelector('.colorBtn');
const bodyBcg = document.querySelector('body');

const colors = ['yellow', 'red', 'green', '#3b5998'];

colorBtn.addEventListener('click', changeColor);

function changeColor (){
    //bodyBcg.style.backgroundColor = colors[2];
    let random = Math.floor(Math.random()*colors.length);
    bodyBcg.style.backgroundColor = colors[random];
}
