
# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
```
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as “menuinandroid″ and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Click option menu and Display menu details give in MainActivity file.

Step 7: Save and run the application.
```

## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by: SRIVARSHAN S
Registeration Number :212221040163
*/
```
```
ACTIVITY_MAIN.XML
<?xml version="1.0" encoding="utf-8"?>
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
```
OPTION.XML
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
```
```
MAINACTIVITY.JAVA
package com.example.menuoption;

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

## OUTPUT
![image](https://github.com/srivarshan123/menuinandroid/assets/103185133/cc7cb4e8-8157-4a3e-a33c-e63f8edb7f2b)
![image](https://github.com/srivarshan123/menuinandroid/assets/103185133/852673e7-98a5-476a-a3d5-4be77cbc479d)
![image](https://github.com/srivarshan123/menuinandroid/assets/103185133/3bad51e1-655a-45ed-afd5-bdb6f095456c)







## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
