# Getting-started-with-windows-forms-using-c#


### Introduction.



**Windows forms** allow the programmers to create a graphical user interface (GUI) that allows the interaction with the program visually. According to [Microsoft](https://docs.microsoft.com/en-us/dotnet/desktop/winforms/overview/?view=netdesktop-5.0) It provides one of the most productive ways to create desktop apps based on the visual designer provided in Visual Studio. Functionality such as drag-and-drop placement of visual controls makes it easy to build desktop apps.


With *windows forms* you can make different types of applications, from basic applications like a calculator and mini-games to high-level applications such as a library database management application that requires the connection of the database to the application.

### Prerequisites.


1. Basic understanding of c# programming language.
2. Visual studio installed on your system.

If you dont have Visual studio installed on your computer. you can download it from [Here](https://visualstudio.microsoft.com/downloads/).

### Make a new project.


In this tutorial, we will make a simple calculator! Make a new project by opening the visual studio, then click on File -> New -> Project -> Visual c# -> Windows desktop and choose Windows Forms App (.NET Framework).


### ToolBox.

The *Toolbox* window provides you with all the controls that help you build your project inside the form. to display the Toolbox click on View -> Toolbox, or you can press Ctrl+Alt+X. To use one of the controls double click on one of them or simply drag and drop it.

### Properties window.

The *Properties window* is used to show the properties of the form or the control that you click on, you can manipulate the properties of any control used in your form. To display the window you can click on View -> properties window or you can simply click F4.   

![Toolbox & Properties window](https://raw.githubusercontent.com/mohamedgh16/Getting-started-with-windows-forms-using-c-/main/properties%20window%20and%20toolbox.png).

### Building the form with the controls.

First of all, let's start with the form and change the text to My calculator. **NOTE:** that changing the name of a Control or the form will only change the name of the object inside the code, and that makes it easier to figure out which button or witch textbox you are using or editing right now, on the other hand changing the text of a Control will only change what appears to the user.

Now let's begin by adding the buttons and the textbox. First, we will add the numbers as buttons then we will add the C button the Calculating button the Operation buttons, and finally, the Textbox that will show the answer.

**NOTE:** dont forget to change both the controls name and the text.

![First_look](https://raw.githubusercontent.com/mohamedgh16/Getting-started-with-windows-forms-using-c-/main/First_look.png).

### Inside the code.

Now let's start coding! First double click on any of the buttons to write your code inside it, let's start with the numbers.

The following code inside each button will add the number to the `Output.Text`.

```c#
 private void Num0_Click(object sender, EventArgs e)
        {
            Output.Text += "0";
        }

        private void Num1_Click(object sender, EventArgs e)
        {
            Output.Text += "1";
        }

        private void Num2_Click(object sender, EventArgs e)
        {
            Output.Text += "2";
        }

        private void Num3_Click(object sender, EventArgs e)
        {
            Output.Text += "3";
        }
        ...
```
Inside the `Dot_Click` we should discuss the case of multiple dots. In order to fix this problem, we should check the the `Output.Text` if it has a dot already inside of it, if not we can normally add a dot to the text.

```c#
          private void Dot_Click(object sender, EventArgs e)
        {
            int Numberofdots = 0;
            for(int i=0;i<(Output.Text.Length);i++)
            {
                if (Output.Text[i] == '.')
                    Numberofdots++;
            }
            if(Numberofdots==0)           
                Output.Text += ".";
        }
```
To clear the `Output.Text` we simply do this.

```c#
private void Cbut_Click(object sender, EventArgs e)
        {
            Output.Text="";
        }
```

Now let's move to the operations.


```c#


```


        













