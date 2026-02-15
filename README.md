
<a href=https://github.com/C0m3b4ck/InputLib-Win32API/blob/main/README_PL.md>🇵🇱🇵🇱🇵🇱🇵🇱🇵🇱POLSKA WERSJA🇵🇱🇵🇱🇵🇱🇵🇱🇵🇱🇵🇱</a>
<br>![GitHub All Releases](https://img.shields.io/github/downloads/C0m3b4ck/InputLib-Win32API/total)
<br><b>🇪🇺🇪🇺🇪🇺Made in Europe🇪🇺🇪🇺🇪🇺
# InputLib-Win32API
A more programmer-friendly library for key input using Win32API, with Win95-Win11 support.
I made this because I plan to use wxWidgets in future projects and am already using it in <a href=https://github.com/C0m3b4ck/SquishyRat>SquishyRat</a>.
# Instructions
<h2><b>Required:</b></h2>
<pre><code>A C++ IDE, I use DevC++ 5.11 with TDM GCC 4.7.3 (GCC needs to be below 4.9)</code></pre>
<pre><code>OPTIONAL: after installation, register DevCPP\MinGW\Bin to PATH</code></pre>

<h2><b>Commands:</b></h2>
<b>Compiling into .dll library:</b>
<pre><code>g++ -c -m32 -D_WIN32_WINNT=0x0400 -DWINVER=0x0400 inputlib.cpp -o inputlib.o
g++ -shared -m32 -D_WIN32_WINNT=0x0400 -DWINVER=0x0400 -static-libgcc -static-libstdc++ -Wl,--out-implib,libkeyinput.a -o inputlib.dll inputlib.o -luser32 -lkernel32
</code></pre>
<b>Outputs: inputlib.dll, inputlib.a</b>
<b>Compiling as .exe (along with other program files)</b>
<pre><code>g++ -m32 -D_WIN32_WINNT=0x0400 -DWINVER=0x0400 main.cpp -L. -inputlib -luser32 -lkernel32 -static-libgcc -static-libstdc++ -o main.exe</code></pre>

# Supported OSes
<b>Supports all versions of Windows, from Windows 95 up to Windows 11:</b>

    Windows 95

    Windows NT 4.0

    Windows 98 

    Windows 98 SE

    Windows 2000

    Windows Me

    Windows XP (tested: x86, x32 and 64-bit, Home, Professional, includes: Starter, Tablet PC, Media Center, Embedded)

    Windows Server (all versions including 2003, Small Business Server 2003, 2003 R2, Home Server,
    2008, Small Business Server 2008, 2012, 2012 R2, 2016, 2019, 2022, 2025)

    Windows Embedded versions, including: Windows Embedded for Point of Service, Windows Embedded Standard 2009, Windows Embedded POSReady 2009

    Windows Vista

    Windows 7

    Windows 8

    Windows 8.1

    Windows 10

    Windows 11

    (probable future desktop OS from Microsoft)

# Author
Original link here: <a href=https://github.com/wxWidgets/wxWidgets/releases/tag/v2.8.8>https://github.com/wxWidgets/wxWidgets/releases/tag/v2.8.8</a>


