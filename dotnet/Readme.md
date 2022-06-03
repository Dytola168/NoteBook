#### Random 
###### C#
```cs
    private void Start_Click(object sender, EventArgs e)
        {
            timer1.Enabled = true;
            
        }
   private void timer1_Tick(object sender, EventArgs e)
        {
            int num2;
            Random mm = new Random();
            num2 = mm.Next(1, 10);
            textBox1.Text = Convert.ToString(num2);
            

        }

        private void button3_Click(object sender, EventArgs e)
        {
            textBox2.Text = textBox1.Text;
            timer1.Enabled =false;
            
        }

```
//new ......................................
#### Sum total return
### box
```cs
    
        private void button1_Click(object sender, EventArgs e)
        {
            text4.Text = (Convert.ToDouble(text2.Text) * Convert.ToDouble(text3.Text)).ToString();
            text5.Text = (Convert.ToDouble(text1.Text) - Convert.ToDouble(text2.Text)).ToString();
        }

        private void button2_Click(object sender, EventArgs e)
        {
            text4.Text = (Convert.ToDouble(text2.Text) / Convert.ToDouble(text3.Text)).ToString();
            text5.Text = (Convert.ToDouble (text1.Text) -Convert.ToDouble( text2.Text)).ToString();
        }

```
##### C#
###### folower time
```cs
@using System.Globalization;

<MudGrid>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="en-US" Variant="Variant.Outlined" Culture="@en" @bind-Value="date" />
    </MudItem>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="de-AT" Variant="Variant.Outlined" Culture="@de" @bind-Value="date"></MudTextField>
    </MudItem>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="cn-ZH" Variant="Variant.Outlined" Culture="@cn" @bind-Value="date"></MudTextField>
    </MudItem>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="en-US: dddd, MMM dd" Variant="Variant.Outlined" Culture="@en" Format="dddd, MMM dd" @bind-Value="date" />
    </MudItem>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="de-AT: dddd, dd. MM." Variant="Variant.Outlined" Culture="@de" Format="dddd, dd. MM." @bind-Value="date"></MudTextField>
    </MudItem>
    <MudItem xs="12" sm="6" md="4">
        <MudTextField Label="cn-ZH: yy年MM月dd日" Variant="Variant.Outlined" Culture="@cn" Format="yyyy年MM月dd日" @bind-Value="date"></MudTextField>
    </MudItem>
</MudGrid>

@code {
    CultureInfo en = @CultureInfo.GetCultureInfo("en-US");
    CultureInfo de = CultureInfo.GetCultureInfo("de-AT");
    CultureInfo cn = CultureInfo.GetCultureInfo("cn-ZH");
    DateTime date = DateTime.Now;
}
```
