Step 1: log into my ieng6 account in the terminal, and you will see something like this:

<img width="819" alt="Screen Shot 2023-05-22 at 5 31 41 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/2973917d-0d7d-493a-91a0-6dff61d8d905">

Step 2: open [lab7](https://github.com/ucsd-cse15l-s23/lab7) in the browser and you will see something like this:

<img width="1302" alt="Screen Shot 2023-05-22 at 5 47 42 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/6af894f2-1c88-42a6-9da7-1da7e0aca183">

Step 3: fork this repository to my github account and open the lab7 and you will see something like this:

<img width="1308" alt="Screen Shot 2023-05-22 at 5 30 20 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/e5ae1b7d-0443-40ad-9b10-158967fa07fb">

Step 4: click on the green bottom that says code and you will see something like this:

<img width="400" alt="Screen Shot 2023-05-22 at 5 30 48 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/da92a13e-632b-46e4-a607-88a47717494c">

Step 5: copy the SSH key and type in "git clone" plus the SSH key and you will see something like this:

<img width="759" alt="Screen Shot 2023-05-22 at 5 39 07 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/b3e98a3a-bb1b-4e71-85b6-3a7452741e3d">

Step 6: use ```<ls>``` command to see what is inside the current repository and type in ```<cd lab7>``` to go to the lab7 file and check what is inside lab7 using ls command like this:

<img width="421" alt="Screen Shot 2023-05-22 at 5 41 43 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/aed1b67b-f9d2-43f6-808e-ca311ff2fb37">

Step 7: check the path of current directory using pwd command like this:

<img width="332" alt="Screen Shot 2023-05-22 at 5 54 29 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/55073680-c04f-46bc-8352-9ec2ed0f823f">

Step 8: from Step 6, we know there is test.sh file that can test the java documents in lab7 and from Step 7, we know the path of lab7. Then we just type in ```<bash test.sh>``` plus the path of lab 7 to test the java files in lab7 and we will see result like this:

<img width="732" alt="Screen Shot 2023-05-22 at 5 57 23 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/001fca5a-ef5a-47cd-ad1e-804d0e0679fd">

Step 9: we found out that there is 1 failure and the merge method in the ListExamples.java document on line 42 went wrong and now we just need to go ahead and fix the issue using vim. We first type in "vim ListExamples.java" to open the java file like this:

<img width="461" alt="Screen Shot 2023-05-22 at 6 03 54 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/496495aa-eb2a-40f4-8d7c-2dd5ca87b2fc">

and we will open up a new window like this:

<img width="642" alt="Screen Shot 2023-05-22 at 6 05 00 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/09507db5-d1f6-4cd8-8bab-4e33289451f8">

Step 10: As prompted by the comment of this code, we just need to change index1 to index2 on line 42 of this file, so we hover over to line 42 and move the cursor until it is on top of "1" and press ```<X>``` to delete the "1" under the cursor like this:

<img width="425" alt="Screen Shot 2023-05-22 at 6 13 10 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/2b39cc33-59ea-403f-9dab-b60664ece3d5">

Step 11: press ```<I>``` on the keyboard to enter the Insert mode and you will see "-- INSERT --" at the bottom of the terminal, which means that you are in the insert mode like this:

<img width="626" alt="Screen Shot 2023-05-22 at 6 15 22 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/ad5be647-95fd-4e03-8beb-0ef206304efb">

Do not move the cursor and type in "2" to fix the bug of this java document like this:

<img width="706" alt="Screen Shot 2023-05-22 at 6 17 20 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/338bb441-580f-46f5-b56e-8cde1005a785">

Step 12: press ```<esc>``` on the keyboard to exit the insert mode and then type in ":wq" and press ```<return>``` on the keyboard to save and exit the vim.

Step 13: now we run the test again the same way we did in Step 8 and we will see that we pass the test like this:

<img width="767" alt="Screen Shot 2023-05-22 at 6 21 11 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/c8263867-227f-4652-b6e2-3a5bbc36f5f4">

Step 14: create a new repository called lab7-result like this:

<img width="1028" alt="Screen Shot 2023-05-22 at 6 41 27 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/9ad98ea8-c21e-4e26-8115-17d5f85584a1">

go into this repository like this:

<img width="1308" alt="Screen Shot 2023-05-22 at 6 42 10 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/7835ef43-cd53-4402-b4e4-23a1ac46c267">

and copy the SSH key.

Step 15: go back to the terminal and type in command "git remote add 123 git@github.com:LipengSheng33/lab7-result.git" and then command "git push 123" and you will see result like this: 

<img width="668" alt="Screen Shot 2023-05-22 at 6 57 10 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/7533be70-2df5-437c-9dfb-023c132d0174">

and you will see your fixed java documents being pushed to the github repository of lab7-result like this:

<img width="1009" alt="Screen Shot 2023-05-22 at 6 59 14 PM" src="https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/9102675a-a627-4554-9b92-90f9ae171421">


