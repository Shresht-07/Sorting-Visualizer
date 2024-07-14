# Sorting-Visualizer
This is a sorting visualizer implements  bubble sort .
const n=20;
const arr=[];
init(); 
function init(){
   for(let i=0;i<n;i++){
       arr[i]=Math.random();
   }
   showBars();  
}


function play(){
    const copy=[...arr]; 
    const moves=bubbleSort(copy);
    animate(moves);
}


function animate(moves){
    if(moves.length==0){
       showBars(); 
       return;
    }
    const move=moves.shift(); 
    const[i,j]=move.indices;
    
    if(move.type=="swap"){
    const temp=arr[i];
    arr[i]=arr[j];
    arr[j]=temp;
    }
    showBars(move); 
    setTimeout(function(){  
        animate(moves);
    },400);
}




 function bubbleSort(arr){
    const moves=[]; 
    for(let i=n-1;i>=1;i--){
        for(let j=0;j<=i-1;j++){
            moves.push ({indices:[j,j+1],type:"compare"});
            if(arr[j]>arr[j+1]){
                moves.push ({indices:[j,j+1],type:"swap"});
                const temp=arr[j];
                arr[j]=arr[j+1];
                arr[j+1]=temp;
            }
        }
    }
  return moves;
} 
function showBars(move){  
    container.innerHTML=""; 
    for(let i=0;i<arr.length;i++){
        const bar=document.createElement("div");
        bar.style.height=arr[i]*100+"%";  
        bar.classList.add("bar");
        if(move && move.indices.includes(i)){
            bar.style.backgroundColor=
               move.type=="swap"?"red":"blue";
        }
        container.appendChild(bar); 
    }
}
