# THR_Program
This Visual Basic Program calculates someones target heart rate.

Public Class Form1

    Private Sub Button1_Click(sender As System.Object, e As System.EventArgs) Handles Button1.Click
        Dim sage As String
        Dim srate As String
        Dim age As Double
        Dim rate As Double
        Dim THR As Double
        sage = txtage.Text
        srate = txtrate.Text
        age = Double.Parse(sage)
        rate = Double.Parse(srate)
        THR = 0.7 * (220 - age) + 0.3 * rate
        txtTHR.Text =
            "Your THR is " & THR.ToString & " beats per minute."
    End Sub

    Private Sub Label4_Click(sender As System.Object, e As System.EventArgs) Handles txtTHR.Click

    End Sub

    Private Sub Form1_Load(sender As System.Object, e As System.EventArgs) Handles MyBase.Load

    End Sub
End Class
