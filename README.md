# Windows

Just some things from me fooling around. Nothing in this repository is to be used for illegal purposes. Strictly for education.

I am not responsible for any actions taken by people borrowing my work. Heck awf :)

I'm attempting to have an hta file connect to a netcat listener via powershell.

The netcat listener then pipes a download cradle into the powershell session.
  Said download cradle pulls a file from my repo here, and initiates a meterpreter session.
  
Thus far, these steps defeat MalwareBytes pro (MBP) subscription, no problem. Running a meterpreter payload on the test system with MBP doesn't work...
  ... but doing a 2-stage approach with a standard shell and immediate upgrade works way better.

As part of the meterpreter session, I have the InitialAutoRunScript running the priv_migrate post module, and have the Unhook option set.
