# How to Disable The Web (Web browsers)

Web browsers (the Web) is an effort to increase accessability of applications to the world. The potential of the Web is quite exciting
with enoumous potential. All major OS vendors have pre-installed browsers by default

## Security Considerations

The Web increases the attack surface of any operating systems that supports it. In security engineering, countermeasures
are typically employed to reduce risk to potential threats. Here are a few concerning aspects of the Web:

* Web server can send web bundles to browser in non-human-readable format
* Web execution relies on browser sandboxing for safety
* Transmission and execution does not require TLS, HSTS, or any other transport layer security mechanism
* Integrity checking is not possible as web apps are not required to be signed by their author
* A primary Web goal is to: *provide developers with useful tools for developing applications*.

Based on the above facts, here are some potential threats in using browsers:

* Static code analysis becomes increasingly difficult as transmitted code may not be human readable
* Sandboxing is prone to breakouts and effectiveness varies largely by implementation. Adobe Flash is an 
example of a technology that was sandboxed after a series of exploits, yet exploits and breakouts still occurred.
* Transmitting over an insecure channel is susceptible  to man-in-the-middle attack. 
* Code signing, the process of verifying software has not been tampered with, is not currently possible with the Web.
The Web is selling itself as the ability to run desktop-like applications in the browser, yet the operating systems
it supports all have code signing requirements for installed software. Allowing random drive-by software to execute
unsigned seems to be a 'feature' of the Web.
* The Web assumes that 'safe applications' can be derived from language subsets and a few rules to prevent 
specific type of behavior. This is similar to blacklisting in the security world, a technique that rarely works.
The specification omits the possibility of misuse cases from their security dialog. Exploits can occur in 'safe applications'
simply by using the application in a way it wasn't designed to run. Since static code analysis is not currently 
possible, automatically identifying potential performance, insider-threats, security, and misuse cases is not possible.

The Web specification does not address any of the above threats. Therefore, I have disabled Web browsers on my personal 
machine and have discountinued use of OSs that do not allow web browsers to be disabled. To be fair, many of the threats 
above also apply to randomly `brew install`ing shit, which **can** be statically analyzed or outright disabled.

## Disabling Guidance

**Windows**

https://www.windowscentral.com/how-remove-microsoft-edge-windows-10


**FireFox**

Drag the *FireFox* icon to the Trash/Recyling Bin

**Chrome/Chromium**

Drag the *Chrome/Chromium* icon to the Trash/Recyling Bin

**Brave**

Drag the *Brave* icon to the Trash/Recyling Bin

**macOS**

macOS does not have advanced functionality and the Developer mode does not have an option to 
uninstall Safari. If someone knows how to uninstall Safari, please submit a pull request.
