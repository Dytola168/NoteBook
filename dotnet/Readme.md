####Random 
###### C#
```cs
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
