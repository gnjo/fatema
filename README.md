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

let d=3dd(mapmacro)
d.uaddr(3,5,1,'e') //x,y,f,v =>X03Y05F01.E
d.move('X00Y00F00.E',0) //like a jump
d.move('E',300) //news ^v<> movetime 300 ms
d.lookup('u',300) //ud news
d.flip(viewcanvas)
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
3dd(`
//symbol=front.png,back.png
//symbol=#000000,#ffffff,
//special transparent => symbol=transparent,#ff00ff
■=wall.png
　=road.png
→=door.png,wall.png
上=upstair.png
下=downstair.png
扉=door.png
出=#ff0000
毒=#ffff00
//size=width,height
//size is floor size. if 41char => 20
size=20,20
■■■■■■■■■■■■■■■■■■■■■■■■■■■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■　■　■　■　■　■　■　■　■　■
■　　　　　　　　　　　　　　■
■■■■■■■■■■■■■■■■■■■■■■■■■■■■
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
`)
```





