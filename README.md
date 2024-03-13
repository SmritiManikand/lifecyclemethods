# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: 212221040157
Registeration Number : 212221040157
*/

XML code:

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
        android:text="HelloWorld"
        android:textColor="#673AB7"
        android:textColorHighlight="#0A1013"
        android:textColorHint="#4A3F3F"
        android:textColorLink="#2F3D43"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.179" />

</androidx.constraintlayout.widget.ConstraintLayout>

JAVA code:

package com.example.lifecycle;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## OUTPUT


## OnCreate

![sh2](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/1b7b54e1-5ade-4217-94e1-47baba875c27)


## OnStart
## OnRestart
## OnPause
## OnStop

![sh1](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/35d97ca1-d702-4a20-88f5-2ab04ba8b0ca)


## OnDestroy



![sh3](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/f348b213-d4b4-4c13-a04b-7a2df7fd5f8a)


![sh4](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/38ab44cd-eb5a-49ce-beed-5edbcbd9f09d)


![sh5](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/efc4a118-9fb4-4207-938c-7eaaecda7d4f)


![sh6](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/54cfe511-fe39-4910-acc2-4cbf1d0c7b18)


![sh7](https://github.com/SmritiManikand/lifecyclemethods/assets/113674204/a316f57f-9857-499f-aeb3-fb9a55d7ab9c)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
