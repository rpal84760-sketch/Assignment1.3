1.Open the terminal:Launch your system terminal:macOS: Press Cmd + Space, type Terminal, and press Enter.Linux: Press Ctrl + Alt + T (or open your distribution's terminal app).Windows: Press Win + X and select Terminal or PowerShell.Move to a convenient working directory such as your Desktop or Documents folder:Bashcd ~/Desktop
2.Create the web-development-practice folder:Create the root project folder and enter it:Bashmkdir web-development-practice
cd web-development-practice
3.Create week-1, week-2, and week-3 subfolders:Create all three weekly directories at once using brace expansion (macOS/Linux/PowerShell 7+):Bashmkdir week-1 week-2 week-3
Verify the folders exist:Bashls -la
4.Create index.html inside each folder:Create an empty index.html file in each subfolder:Bashtouch week-1/index.html week-2/index.html week-3/index.html
(In Windows PowerShell, you can use New-Item -Path week-1\index.html, week-2\index.html, week-3\index.html -ItemType File.)Check your directory tree:Bashfind . -maxdepth 2 -ls
5.Practice navigating, renaming, and deleting folders:Practice moving around, renaming a directory with mv, and removing a test directory with rm -r:Bash# Navigate into week-1 and back out
cd week-1
pwd
cd ..

# Create a temporary folder, rename it, then delete it
mkdir temp-practice
mv temp-practice renamed-practice
rm -r renamed-practice
(Be careful with rm -r—always double-check the target folder name before pressing Enter.)6.Open the project folder in VS Code from the terminal:Make sure you are inside web-development-practice, then launch VS Code pointing to the current directory (.):Bashcode .
If code is not recognized on macOS, open VS Code, press Cmd + Shift + P, run Shell Command: Install 'code' command in PATH, and try again.