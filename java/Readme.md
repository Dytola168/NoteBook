#### Java
##### main class
``` java    
// in main.java...................
public class Class_1 {

    public static void main(String[] args) {
        IPhone wk = new IPhone("tes","IPhone11",100,"red","verson 12");
        wk.showData();

    }
     
}
        
```
### extends
```java
    // in Phone.java...................
    package class_1;

public class Phone {
   public String IME;
   public String Model;
    float Price;
   public String Color;
   public Phone(){
   }
   public Phone(String IME,String Model,float Price,String Color){
       this.IME = IME;
       this.Model= Model;
       this.Price = Price;
       this.Color =Color;
   }
   public void showData(){
       System.out.println("IME :"+IME);
       System.out.println("MOdel :"+Model);
       System.out.println("Price :"+Price);
       System.out.println("Color :"+Color);
   
   }
    
}
   // Iphone.java....................................................
    package class_1;
class IPhone extends Phone {
    public String ios_verson;
    public IPhone(String IME,String Model,float Price,String Color,String ios_verson){
    super(IME,Model,Price,Color);
    this.ios_verson=ios_verson;
    
    }
    public void showData(){
        super.showData();
        System.out.println("ios-verson :"+ios_verson);
    }
    
}
```
#### FORM 
```js
private void btSumActionPerformed(java.awt.event.ActionEvent evt) {                                      
        float v1,v2,result;
        v1=Float.parseFloat(textBox1.getText());
        v2=Float.parseFloat(textBox2.getText());
        result=v1+v2;
        textResult.setText(result+"");
    }                                     


```
