<html>
<head>
    <meta charset="utf-8"/>
</head>
<body>
    <input id="up" style="position:fixed;font-size:30px;" onclick="upf()" type="button" value="^">
    <input id="down" style="position:fixed;font-size:30px;transform:rotate(0.5turn);" onclick="downf()" type="button" value="^">
    <input id="right" style="position:fixed;font-size:30px;" onclick="rightf()" type="button" value=">">
    <input id="left" style="position:fixed;font-size:30px;" onclick="leftf()" type="button" value="<">
    <div id="pp" style="position:fixed;font-size:30px;">原神啟動</div>
    <script>"use strict";
        setInterval(function(){},3000);
        let cp=pp.getBoundingClientRect();
        pp.style.left=0+"px";
        pp.style.top=document.documentElement.clientHeight-cp.height+"px";
        let u=up.getBoundingClientRect();
        up.style.left=document.documentElement.clientWidth/2-u.width/2+"px";
        up.style.top=document.documentElement.clientHeight/2-u.height/2+"px";
        let r=right.getBoundingClientRect();
        right.style.left=document.documentElement.clientWidth/2+r.width/2+"px";
        right.style.top=document.documentElement.clientHeight/2-r.height/2+"px";
        let l=left.getBoundingClientRect();
        left.style.left=document.documentElement.clientWidth/2-l.width*3/2+"px";
        left.style.top=document.documentElement.clientHeight/2-l.height/2+"px";
        let d=down.getBoundingClientRect();        
        down.style.left=document.documentElement.clientWidth/2-d.width*5/2+"px";
        down.style.top=document.documentElement.clientHeight/2-d.height/2+"px";
        let y=document.documentElement.clientHeight-cp.height;
        let x=0;
        function upf(){
            y-=10;
            pp.style.top=y+"px";
        }
        function rightf(){
            x+=10;
            pp.style.left=x+"px";
        }
        function leftf(){
            x-=10;
            pp.style.left=x+"px";
        }
        function downf(){
            y+=10;
            pp.style.top=y+"px";
        }
        import {ji} from './read.md';
        if(confirm("dipt")){
            alert(ji);
            //localStorage.setItem("test",+localStorage.getItem("test")+1);
            //alert(localStorage.getItem("test"));
        }
        else{
            alert(ji);
            //alert(localStorage.getItem("test"));            
        }
    </script>
</body>
</html>
