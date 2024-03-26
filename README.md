Choice = "Y"
Pi = 3.14159
While (Choice <> "X")
menu()
If Choice <> "A" and Choice <> "C" and Choice <> "X" Then
Choice = "Err"
EndIf
If Choice = "A" then
AreaOfCir()
EndIf
If Choice = "C" then
CircOfCir()
EndIf
If Choice = "Err" Then
TextWindow.Clear()
TextWindow.WriteLine("Bad Parameter. Try Again.")
TextWindow.Write(Type the letter N and press enter to continue.....”)
NextUp = TextWindow.Read()
EndIf
TextWindow.WriteLine("O.K.")
EndWhile
'End of Program
'Calculation Subroutines Start Here
sub menu
TextWindow.Clear()
TextWindow.WriteLine(" ")
TextWindow.WriteLine(" Menu")
TextWindow.WriteLine(" ")
TextWindow.WriteLine("Select the calculation from the list below (Use Caps)")
TextWindow.WriteLine(" ")
TextWindow.WriteLine("A - Area of a Circle")
TextWindow.WriteLine("C - Circumference of a Circle")
TextWindow.WriteLine(" ")
TextWindow.WriteLine("X - Exit")
Choice = TextWindow.Read()
EndSub
Sub CircOfCir
TextWindow.Write(“Type the letter N and press enter to continue.....”)
NextUp = TextWindow.Read()
EndSub
Sub AreaOfCir
TextWindow.Write(“Type the letter N and press enter to continue.....”)
NextUp = TextWindow.Read()
EndSub
