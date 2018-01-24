# cookie

## JS获取cookie

```javascript
cookie 是document的属性
document.cookie = '';
// 保存cookie  -- 设置时间


// 设置 cookie
function setCookie(keys,values,time){
  if(time){
    let date = new Date;
    date.setTime(date.getTime()+time*1000*60*60);
    document.cookie = keys + "=" + values + ";expires=" + date.toGMTString;
  }else{
    document.cookie = keys + "=" + values;
  }
}


// 删除cookie  
function deleteCookie(keys){
  let date = new Date;
  date.setTime(date.getTime()-1000);
  document.cookie = keys +'=aa;expires='+date.toGMTString();
}
 
// 获取cookie

function getCookie(keys){
  let arr = document.cookie.split(';');
  for(let i=0;i<arr.length;i++){
    let newarr = arr[i].split('=');
    if(newarr[0] == keys){
      return newarr[1];
    }
  }
  return '没有';
}

```















