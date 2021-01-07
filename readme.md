# Enable Cortana (Microsoft Eva Mobile) TTS voice 

This guide enables the TTS voice for Microsoft Eva Mobile (En-US, Female) for all win32 apps. The scripts and registry edits are provided as is and no guarantuees are provided for the instructions here. 

## Prerequisites

* You need to change your Windows 10 language to English (US) to enable Cortana availability. 
* You need to setup Cortana (Windows Settings or Windows Cortana App) with English (US).

Go to `C:\Windows\Speech_OneCore\Engines\TTS\en-US\` to check that there are 9 files that start with '`M1033Eva`'. If they cannot be found, check again that Cortana is avaiable.  

## How-to

1. Click on `Microsoft-Eva-Mobile.reg` to add the Eva Mobile voice to the registry.
2. Restart your computer. 
3. Open a PowerShell window (< PowerShell 7) as admin and copy all of `Test-TTS-voices.txt` into the PowerShell window to test all available voices.

Additionally, other mobile voices found in `C:\Windows\Speech_OneCore\Engines\TTS\en-US\` can be enabled by copying the scipts from `Enable-mobile-voices.txt` to an admin PowerShell window. This may be broken since Cortana has been decoupled from the system in update 20H1. 

Scripts and guide by [u/Pessimist__Prime](https://www.reddit.com/r/EliteDangerous/comments/5d02vv/if_you_use_voiceattack_eddi_or_any_other/) and [@jpoon](https://gist.github.com/jpoon/d926243f19642b04f1a6).
