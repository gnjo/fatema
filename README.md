# fatema
```
#start

{{{

}}}

{{{js
//multiline javascript world
//but need use
}}}

#start.loop
k>
w>100 //wait 100 msec
$wk=($$k==='a')?console.log($$k,'a'):console.log($$k,'other key')


{1}>>>#start.loop

//command
{{{ }}}
js>$$$
k>
w>
#start
$wk=console.log('xyz')
{1}>>>#start

```
```
toBig()
toSmall()
```



```

//
d.x
d.y
d.f
d.v
d.addr
//
//天井の描画はない。上り階段と下り階段は、壁に描く。
//床の状態は重ねない。毒の床の上で、イベントを設置できなくなるが、簡略化の為。
//！ event the person
//？ event the object, switch, chest, key.
//

```

```
let d1=3dd(`
//walls/////////////////////////////////////////////////////////
//symbol=front.png,back.png
//symbol=#000000,#ffffff
//special transparent is single #=> symbol=#,#ff00ff
////
■=wall.png
→=door.png,wall.png
上=upstair.png
下=downstair.png
扉=door.png
出=#ff0000
//grounds//////////////////////////////////////////////////////
//symbol=ground.png
//！=#000000
////
　=#000000
毒=#ffff00,#000000
//grounds with standing object////////////////////////////////////////////
//symbol=man.png
//カタカナのアからンまで。濁点は非推奨。
ア=xxxx.png
//size is floor size. if 41char => 20
//need head Fxx=
F01=
■■■■■■■■■■■■■■■■■■■■■■■■■■■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■■■■■■■■■■■■■■■■■■■■■■■■■■■■
F02=
■■■■■■■■■■■■■■■■■■■■■■■■■■■■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■■■■■■■■■■■■■■■■■■■■■■■■■■■■
//always trim and // 
`).test()
;

function tick(){
  requestAnimationFrame(tick);
   if(!d1.loading)
    if(d1.show)
     if(d1.moving)
      dung1.flip(canvas)
}

d1.move(1,1,1,'E',movetime)//f,x,y,e,movetime
d1.move('F01X01Y01.E',0) //like a jump
d1.move(20,20,300) //x,y,movetime
d1.gets('F01X01Y01.E')//other pos
d1.gets() //now pos
d1.move('E',300) //news ud ^v<> movetime 300 ms
d1.move('^',300) //foward
d1.move('u',300) //up stair if F02 => F01
d1.lookup('u',300) //ud news
d1.flip(viewcanvas)

//d1.automove(baseaddr,moves,span,maxstep)
//d1.automove('F01X01Y01.E','>>>>>^^^^^^^^>>>>>>>^^^^^^',300)
//d1.automove(baseaddr,walls,span,maxstep)
d1.automove('F01X01Y01.E','■',300,255)
//algorithm right and left touch 

```

```
 function lex(text){
  let o={};
 }
let 3dd=function(text){
 let o={}
 o.canvas=document.createElement('canvas')
 o.fdata=Array.from({length:10})
 ;
 o.move=function(){
 }
 o.gets=function(){
 }
 o.flip=function(viewcanvas){
  
 }
}

```


