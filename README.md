# NoteBook
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
> extends
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
#### GIT
##### branch
```shell
git push origin HEAD:dytola
```
#### C# Random
```cs
private void timer1_Tick(object sender, EventArgs e)
        {
            int num2;
            Random mm = new Random();
            num2 = mm.Next(1, 10);
            textBox1.Text = Convert.ToString(num2);
            

        }
```
#### URL GIT
```js
    describe('parse(url)', function () {
  it('should support git://*', function () {
    var url = 'git://github.com/jamesor/mongoose-versioner'
    parse(url).should.equal('https://github.com/jamesor/mongoose-versioner')
  })

  it('should support git://*.git', function () {
    var url = 'git://github.com/treygriffith/cellar.git'
    parse(url).should.equal('https://github.com/treygriffith/cellar')
  })

  it('should support https://*', function () {
    var url = 'https://github.com/Empeeric/i18n-node'
    parse(url).should.equal('https://github.com/Empeeric/i18n-node')
  })

  it('should support https://*.git', function () {
    var url = 'https://jpillora@github.com/banchee/tranquil.git'
    parse(url).should.equal('https://github.com/banchee/tranquil')
  })

  it('should return undefined on failure', function () {
    var url = 'git://github.com/justgord/.git'
    assert(parse(url) == null)
  })

  it('should parse git@github.com:bcoe/thumbd.git', function () {
    var url = 'git@github.com:bcoe/thumbd.git'
    parse(url).should.eql('https://github.com/bcoe/thumbd')
  })

  it('should parse git@github.com:/bcoe/thumbd.git', function () {
    var url = 'git@github.com:/bcoe/thumbd.git'
    parse(url).should.eql('https://github.com/bcoe/thumbd')
  })

  it('should parse git@github.com:bcoe/thumbd.git#2.7.0', function () {
    var url = 'git@github.com:bcoe/thumbd.git#2.7.0'
    parse(url).should.eql('https://github.com/bcoe/thumbd')
  })

  it('should parse git+https://github.com/bcoe/thumbd.git', function () {
    var url = 'git+https://github.com/bcoe/thumbd.git'
    parse(url).should.eql('https://github.com/bcoe/thumbd')
  })

  it('should parse git+ssh://github.com/bcoe/thumbd.git', function () {
    var url = 'git+ssh://github.com/bcoe/thumbd.git'
    parse(url).should.eql('https://github.com/bcoe/thumbd')
  })

  it('should parse https://EastCloud@github.com/EastCloud/node-websockets.git', function () {
    var url = 'https://EastCloud@github.com/EastCloud/node-websockets.git'
    parse(url).should.eql('https://github.com/EastCloud/node-websockets')
  })

  // gist urls.

  it('should parse git@gist urls', function () {
    var url = 'git@gist.github.com:3135914.git'
    parse(url).should.equal('https://gist.github.com/3135914')
  })

  it('should parse https://gist urls', function () {
    var url = 'https://gist.github.com/3135914.git'
    parse(url).should.equal('https://gist.github.com/3135914')
  })

  // Handle arbitrary GitHub Enterprise domains.

  it('should parse parse extra GHE urls provided', function () {
    var url = 'git://github.example.com/treygriffith/cellar.git'
    parse(
      url, {extraBaseUrls: ['github.example.com']}
    ).should.equal('https://github.example.com/treygriffith/cellar')
  })

  it('should parse GHE urls with multiple subdomains', function () {
    var url = 'git://github.internal.example.com/treygriffith/cellar.git'
    parse(
      url, {extraBaseUrls: ['github.internal.example.com']}
    ).should.equal('https://github.internal.example.com/treygriffith/cellar')
  })
})

describe('re', function () {
  it('should expose GitHub url parsing regex', function () {
    parse.re.source.should.equal(
      /^(?:https?:\/\/|git:\/\/|git\+ssh:\/\/|git\+https:\/\/)?(?:[^@]+@)?(gist.github.com|github.com)(?::\/?|\/)([^/]+\/[^/]+?|[0-9]+)$/.source
    )
  })
})

```
#### C#
##### Code color BG
```cs


<MudPaper Class="pa-4" Style="@($"color:{Colors.Purple.Accent3};")">
    Colors.Purple.Accent3
</MudPaper>
<MudPaper Class="pa-4" Style="@($"color:{Colors.LightGreen.Accent3}; background:{Colors.BlueGrey.Darken4};")">
    Colors.BlueGrey.Darken4 Colors.LightGreen.Accent3
</MudPaper>



```
