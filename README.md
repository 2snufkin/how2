# Angular

##how to force element into focus
- verify that the element has focus att. 
- create a temlate ref in the html. let's say it's name is inp
```ts
  @ViewChild('inp') inputEle: any; 

    ngAfterViewChecked(){
      if(this.inputEle){
           this.inputEle.nativeElement.focus();
      }
```
----------------------------------
