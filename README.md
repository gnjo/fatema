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
//symbol=ground,groundback,pointlightcolor
//！=#000000,#000000,#ff0000
////
　=#000000
毒=#ffff00,#000000
////////////////////////////////////////////////////////////////
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
d1.gs('E') //getsymbol
d1.gs('F01X01Y01.E')//
d1.gs() //now ground
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

let moving=0
function chase(target,camera,ofs){
  var relativeCameraOffset = new THREE.Vector3(ofs[0],ofs[1],ofs[2]);
	var cameraOffset = relativeCameraOffset.applyMatrix4( target.matrixWorld );
	camera.position.x = cameraOffset.x;
	camera.position.y = cameraOffset.y;
	camera.position.z = cameraOffset.z;
	camera.lookAt( target.position );  
 }
}
function rot(target,deg,time){
 moving=1
 time=time||300
 let s=10,dd=THREE.Math.degToRad(deg/s),dt=time/s,i=0
 let id=setInterval(()=>{
  if(i>s) clearInterval(id),moving=0
  target.rotateOnAxis( new THREE.Vector3(0,1,0),dd);  
  i++
 },dt)
}


```


