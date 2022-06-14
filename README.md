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

