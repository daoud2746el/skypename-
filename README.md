# skypename-
#include &lt;SkypeCOM.au3>  _SkypeCOM_StartClient() ; starts Skype if it isn't running ; you may need a sleep() timeout here to allow time for Skype to sign your account in before the script proceeds... I'm working on a way to get around this. You don't even need to use the StartClient() function if you already have Skype open and logged in  If _SkypeCOM_Attach() Then ; attempts to attach to Skype if the attachmentstatus is not Success     _SkypeCOM_PlaceCall("+18005555555", "echo123") ; you can use a number, skypename or speed dial code Else     MsgBox(48,"Error","Unable to attach to Skype.") EndIf
