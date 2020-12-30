# BSGS
Baby Step Giant Step Combined Efforts to Find 1.2 Bitcoin

I have tweaked the code of Jean Luc Pons' Baby Step Giant Step program ( https://github.com/JeanLucPons/BSGS ) to help find the #120 puzzle in the Bitcoin Challenge Transaction ( https://bitcointalk.org/index.php?topic=5218972.0 ).

Not everyone has a GPU or a high powered GPU to use programs such as Bitcrack or Kangaroo methods. But mostly everyone has a CPU, and that is what powers the Baby Step Giant Step (BSGS) program...the CPU located in your computer. Now, everyone has a chance to help crack the puzzle. One major advantage over Kangaroo methods, the BSGS is easy to give different ranges to workers without losing in complexity which is not possible with Kangaroo.

Download the exe files and batch files here:
https://github.com/WanderingPhilosopher/BSGS

The tweaks I made to the original code include:
a random range generator
the program now automatically creates the input file:
Baby Step Size
Start Range
End Range
and applicable Public Keys (to search for)

All you have to do is download the tweaked program and the already made batch file. Once you download the files, place them in the same folder and double-click on the batch file. The program will automatically start searching for the public key. That's it. It's that easy.

What you will notice in the folder you placed your files in:
an input file will automatically pre-fill
and there will be a file called ranges_searched.txt

After we run the program for awhile, people can send me their ranges_searched.txt file and I can keep track of ranges searched and maybe this will help us narrow down to a smaller range in the future. Or, people can post how many ranges they've already searched and we can keep a running tally.

I took the #120 public key (120 bits) and compressed it down to 117 bits to make our search range 8 times smaller.

What happens when you find the public key?
If your CPU finds a key, a text document called, FOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYSFOUNDKEYS.txt will be created in the folder and it will contain the private key and the public key. Send that information to me, along with your bitcoin wallet address, and I will recreate the original #120 public key, and we will split the 1.2 bitcoin 50/50. It's that easy.

How I am running the program on my computer:
I have downloaded the 16 BSGS exe files and the 16 batch files. In each batch file, it calls to use one CPU thread (-t 1). So I run as many as the batch files/programs as my CPU can handle. On an i5-4690, with four instances running (4 threads total), each thread completes a range in about 9 seconds. So that's 4 ranges checked every 9 seconds, which on the safe side, this one computer checks about 34,560 ranges a day. Let me know how fast your computer completes a range.
