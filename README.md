# -C-Encode-and-Decode-HTML
[C#] Hướng dẫn Encode and Decode HTML
```C#
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Net;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace HTMLEncodeDecode
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void btnEncode_Click(object sender, EventArgs e)
        {
            var inputText = txtInput.Text.Trim();
            var htmlEncode = WebUtility.HtmlEncode(inputText);
            txtOutput.Text = htmlEncode;
        }

        private void btnDecode_Click(object sender, EventArgs e)
        {
            var inputText = txtInput.Text.Trim();
            var htmlDecode = WebUtility.HtmlDecode(inputText);
            txtOutput.Text = htmlDecode;
        }
    }
}
```
