# Form2_TPTRABALHO
.---
    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click
        Dim i As Integer
        For i = 0 To info.length - 1
            If info(i).nome = TextBox1.Text And TextBox2.Text = "" And TextBox3.Text = "" And TextBox4.Text = "" And ComboBox1.SelectedIndex = -1 Then
                'For Each nome As ListViewItem In ListView1
                ListView1.Items.Add(New ListViewItem({info(i)}))
            End If
        Next
        
                For i = 0 To info.length - 1
            If info(i).nome = "" And TextBox2.Text = "" And info(i).data.month = TextBox3.Text And TextBox4.Text = "" And ComboBox1.SelectedIndex = -1 Then
                cont += 1
                ListView1.Items(cont).SubItems(1).Add(info(i).data.month)
            End If
        Next
    End Sub
    End Sub

'pesquisar
    For Each jogador In info
        newitem = New ListViewItem(info(jogador.nome))
        newitem.SubItems.Add(info(jogador.escalao))
        newitem.SubItems.Add(info(jogador.data.ToString))
        newitem.SubItems.Add(info(jogador.chs))
        Listview2.Add(newitem)
        cont = jogador.nome.IndexOf(Form2.Txt_Nome.Text, contador)
        
        
        
Form1 
'Pesquisar
    For each jogador in info
        newitem =  New ListViewItem(info(info.indexof(jogador).nome)
        newitem.SubItems.Add(info(info.indexof(jogador).data.year)
        newitem.SubItems.Add(info(info.indexof(jogador).data.month)
        newitem.SubItems.Add(info(info.indexof(jogador).data.day)
        newitem.SubItems.Add(info(info.indexof(jogador).escal)
        
        
        
        
        
        
        
        
        
        
        
'Pesquisar_ORIGINAL_Form1
    Dim newitem As ListViewItem
         For Each jogador In info
            newitem = New ListViewItem(info(Array.IndexOf(info, jogador)).nome)
            newitem.SubItems.Add(info(Array.IndexOf(info, jogador)).data.Year)
            newitem.SubItems.Add(info(Array.IndexOf(info, jogador)).data.Month)
            newitem.SubItems.Add(info(Array.IndexOf(info, jogador)).escal)
         Next
    
Pesquisar_ORIGINAL_Form2
Btn_depesquisa.Click()
        filtro(TextBox1.Text.Text, 0)
        filtro(Combobox1.Text.Text, 1)
        filtro(TextBox2.Text.Text, 2)
        filtro(TextBox3.Text.Text, 3)
        filtro(TextBox4.Text.Text, 4)
        PictureBox1.Image =  Form1.info.IndexOf(TetxBox1.Text).imagem
End Sub   
   
   
   
   
   
-FUNCTIONS
(FORM2)
    Sub org(string As String, index As Integer)
        Dim i as Integer
        
        i = 0
        If string <> "" Then
            For i = 0 To ListView1.Items.Count - 1
                If ListView1.Items(i).SubItems(index).Text.IndexOf(string) = -1 Then
                    ListView1.Items.RemoveAt(i)
                End If
            Next
            c = 0
        End If
    End Sub
