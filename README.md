# kaina
const puppeer=require('puppeteer')
asyn funtion run(){
const browser=await puppeteer.launch()
const page=await browser.newPage()
await page.goto('https://platzi.com/cursos/html5-css3/opiniones/1/')
await page.screeshot({
path:'screenshot.png',
fullPage true,})

}
run()
