# Ex.No:10 To create a option menu to display menu items.
# AIM:
 To create a option menu to display menu items.

# EQUIPMENTS REQUIRED:
Latest Version Android Studio

# ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project. 
Step 2: Then type the Application name as “option menu” and click Next. 
Step 3: Then select the Minimum SDK as shown below and click Next. 
Step 4: Then select the Empty Activity and click Next. Finally click Finish. 
Step 5: Design layout in activity_main.xml. 
Step 6: Get contacts details and Display details give in MainActivity file. 
Step 7: Save and run the application..

# PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:DIVYASHREE B S
Registeration Number :212221040044
*/
```
# activity_main.xml
```
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
# MainActivity.java
```
package com.example.optionmenu;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
```
# option.xml
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
```
# OUTPUT
![image](https://github.com/Poojariyaa/optionmenu/assets/127511817/977240ce-58dd-4067-9a2c-f03f29fe5ec0)
![image](https://github.com/Poojariyaa/optionmenu/assets/127511817/f803878d-0718-498a-89f5-4e2f4582bab7)
![image](https://github.com/Poojariyaa/optionmenu/assets/127511817/cec8b94c-fa84-4de3-a62c-b86144e87145)
![image](https://github.com/Poojariyaa/optionmenu/assets/127511817/1736912d-f1b1-433d-85e0-fc5c7ffc5e88)


# RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
