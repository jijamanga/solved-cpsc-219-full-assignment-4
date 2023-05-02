Download Link: https://assignmentchef.com/product/solved-cpsc-219-full-assignment-4
<br>
Text only connections such as Putty won’t allow you to run programs that employ graphical user interfaces. If you have been working at home to complete assignments but haven’t installed JDK on your computer then you might want to [<a href="http://pages.cpsc.ucalgary.ca/~tamj/resources/drivemapping.pdf">map your UNIX account</a>] to a drive on your computer.You can then access all the files on your computer science account directly from your home computer and use whatever editor that you wish. If you open up a remote connection using Putty then you can still compile your programs but it will be with the CPSC compilers. Finally to run your programs you can run ‘Java’ locally using JRE (unlike the JDK which includes the compiler you don’t have to worry about setting the classpath). Open up a command line on your home computer ‘cmd’ and use it to navigate to where you have your GUI code on your CPSC account. (Don’t forget to change drives – the drive letter will be whatever letter that you used when you initially mapped a drive to your UNIX account). When you type ‘java Driver’ (or whatever the name of starting class is) your GUI will be run locally on your computer.

<h3><strong>New concepts to be applied for this assignment:</strong></h3>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li>Implementing a graphical user interface</li>

   <li>File output (using FileWriter and PrintWriter)</li>

   <li>Exceptions</li>

  </ul></li>

</ul>




<strong>Description</strong>

Implement a simple graphical user interface to simulate a shopping program. You have some flexibility in the exact content and layout, an example is shown in Figure 1.

<table width="100%">

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td><strong>Figure 1</strong>: Main shopping screen</td>

  </tr>

 </tbody>

</table>

At a minimum this window should consist of the following: a JFrame container, a JTextField and JTextArea for the name and address input areas (respectively), Jlabels to describe the input fields, two JButtons to handle most of the user interaction. The full version of the program will employ the GridBagLayout (and GridBagConstraints) for the main shopping window (it’s optional for the login dialog). Regardless of whether a layout ‘manager class’ is used the layout should be organized and logical so the user can quickly understand the interface at a glance. If you desire you can use other sub-containers with other layout manager classes. ImageIcons will be used to adorn the buttons (your choice of image but it should complement the text descriptions).  Finally you should include another image somewhere in the container with an appropriate company logo (“TAMCO Enterprises Inc.” in the example) contained with a Java GUI Component (a JLabel is a good choice). There should be an appropriate descriptive title in the window. If you use external data – something that you didn’t create yourself – unless it’s largely in the public domain (e.g., clipart that is made universally available for free) make sure that you cite the source. The program should be written so that the data files (order file and images) will reside in the same directory as your program (so your marker doesn’t have to waste time determining the structure assumed…those few minutes adds up over the course of marking all the assignments in a tutorial).

<ol>

 <li><strong>Save button</strong>: When pressed this button will take the current information in the name and address and save it to a plain text file (unencrypted) called ‘order.txt’ which should be saved in the same directory as your program. The name information should sit by itself on the first line of the file while the second line (and successive lines – if appropriate) will consist of the address. Each line of the address from the JTextArea will reside on a separate line in the order file (the example shown in Figure 1 will create a order file with 4 files: 1 for the name and 3 for the address). If you are still unsure then you should look at the sample order file ‘order.txt’ in the A5 directory. It’s the result of saving the order shown in Figure 1. The program does not have to read this information from the file. (You only have implement file output not input). If the file already exists then the previous contents can be overwritten. During the save process the title bar of the main window should provide an appropriate status message (and the program should temporarily pause itself to provide the user with enough time to read it).</li>

 <li><strong>Clear button</strong>: When pressed the two input fields (name and address should be cleared of text).</li>

</ol>

As previously indicated clicking on the close window control will just shut the application down. Because the address field can consist of multiple lines (i.e., the user can hit enter to separate lines) hitting enter in the name field should have no effect (unlike the password field).In the assignment directory (<a href="http://pages.cpsc.ucalgary.ca/~tamj/2016/219W/assignments/assignment4/assignment4/data">/home/219/assignments/assignment4/data</a>) there will be sample images that you can use in your program, a sample ‘order.txt’ file.You may also find in this directory a short video illustrating how my sample solution works. Keep in mind that this year’s version of the assignment has been reduced slightly in size so the video includes additional features such as a login dialog and password encryption that you don’t have implement. As well the sound effects that are triggered when the mouse ‘enters’ the label aren’t necessary either.

<table width="100%">

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td>Video: Running my sample solution (“.wmv” format). AGAIN: it contains a few extra features over and above what you need for this years version.</td>

  </tr>

 </tbody>

</table>

<h4><strong>Using pre-written Java code</strong></h4>

Unlike the other assignments you will make extensive use of the pre-created Java libraries developed by Sun/Oracle for graphical components (e.g., java.awt., javax.swing), event handling (e.g.,java.awt.event) and the two classes for file output.

<ul>

 <li></li>

 <li><strong>Data files</strong></li>

 <li><strong>How the interactive widgets work</strong></li>

 <li>Description:</li>

</ul>