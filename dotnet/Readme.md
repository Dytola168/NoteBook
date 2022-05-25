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
