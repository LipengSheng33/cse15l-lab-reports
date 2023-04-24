Lab report 1

Step 1: Search “VScode download” on Google and click on the official VScode website at https://code.visualstudio.com/download, which will look like this:
![image](https://user-images.githubusercontent.com/130394449/233861743-bd3a43b9-0674-4b21-a97d-af8ed3a0964e.png)

Step 2: Click on the correct download button based on the operating system on your computer. Download and install the VScode. After successfully installed the VScode, open the VScode and it will look like this:
![image](https://user-images.githubusercontent.com/130394449/233861820-d700831c-9299-4cfa-bb1a-0c7c2891a218.png)

Step 3: Find your CSE15L account in this link: https://sdacs.ucsd.edu/~icc/index.php, look up your cse15l course account by typing in your UCSD student username and student ID and click on submit. The username that starts with "cs15lsp23" is your CSE15L account. Then you need to reset your password at https://password.ucsd.edu/GetUser.aspx by typing in your CSE15l account your just looked up in the "Enter your username:" box, clicked on continue, click on "I want to reset my course-specific account password, click on "yes" on the page that says "confirm your email address" and you will receive an instruction on how to reset your password in your school email. 

Step 4: Open your terminal in VSCode and type “ssh “+ your account+”@ieng6.ucsd.edu” and push the return button on your keyboard. You will see this:

![Capture1](https://user-images.githubusercontent.com/130394449/234067005-04b4452c-48de-4e9e-8d8e-1ed8e8f5f07d.PNG)

Then type “yes” and push the return button. They will ask you to enter your password like this:
![Capture](https://user-images.githubusercontent.com/130394449/234067061-5939c00c-baa5-458f-b401-39be96ea132b.PNG)

Then typed the password of your CSE15L account and push the return button. You will see something like this:
![Capture2](https://user-images.githubusercontent.com/130394449/234067137-dcc2d46f-e06f-4592-ab2a-6795d847923b.PNG)

I did not get my password right at first, so the terminal keeps asking me to enter password again and again. Finally I get my password right and I get the message that inform me how many failed attempts I have as shown in the image above.

Step 5: Try some command in your terminal such as “cd ~”, “cd”, “ls -lat” and “ls -a”. Push the enter button on your keyboard each time you complete a command. You will see the output of your command in your terminal just like this:
![image](https://user-images.githubusercontent.com/130394449/233861926-11216c1f-6f5f-45c2-aff4-f0901dddcd50.png)

Try some more command such as "cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/" and "cat /home/linux/ieng6/cs15lsp23/public/hello.txt". You will see something like this:
![Capture3](https://user-images.githubusercontent.com/130394449/234068958-4d5028e3-e340-4f8d-89bf-736450d8d706.PNG)
The "cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/" command copy the hello.txt file to the remote filesystem and the "cat /home/linux/ieng6/cs15lsp23/public/hello.txt" read the file and print out the content of the file.
