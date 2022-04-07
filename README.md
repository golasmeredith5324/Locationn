# Locationn
ConsoleWrite ("! EmpInventory.exe not found" &amp; @CRLF) EndIf  Local $oShell = ObjCreate("shell.application") Local $oShellWindows = $oShell.windows  If IsObj($oShellWindows) Then     $string = ""     For $Window In $oShellWindows         $string = $string &amp; $Window.LocationName &amp; @CRLF     Next     MsgBox(0, "", "Your Current Open Shell Windows:" &amp; @CRLF &amp; $string)
