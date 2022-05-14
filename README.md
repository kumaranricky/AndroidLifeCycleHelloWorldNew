# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:
Android Studio(Min.required Artic Fox)

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:

/*
Program to print the text “Hello World”.\
Developed by:Kumaran.B\
Registeration Number :212220230026\
*/

## activity_main.xml
```xml

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout 
             xmlns:android="http://schemas.android.com/apk/res/android"
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
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```java
package com.example.lifecycle;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(),
                       "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(),
                      "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(),
                      "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(),
                        "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(),
                          "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(),
                            "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), 
                             "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```


## <br/><br/><br/><br/><br/><br/><br/><br/><br/>OUTPUT:
![create](https://user-images.githubusercontent.com/75243072/165220565-b60cdf6e-e1de-47b5-8e08-335c398cd870.png)

![start](https://user-images.githubusercontent.com/75243072/165220664-d2808a80-961c-4e7f-969e-3044427e79b6.png)

![stop](https://user-images.githubusercontent.com/75243072/165220966-4dcfe574-27bb-4fe7-bb17-4afc1325cd99.png)

![resume](https://user-images.githubusercontent.com/75243072/165221096-4fcc9378-c5fb-47b3-ac92-3f1a52a59291.png)

![pause](https://user-images.githubusercontent.com/75243072/165220975-b055acac-f8f8-43d7-90d4-1951e493b59f.png)

![restart](https://user-images.githubusercontent.com/75243072/165220979-2bec9407-e748-496e-801c-001b96a1f3bc.png)

![destroy](https://user-images.githubusercontent.com/75243072/165220969-8e64dc1d-62ae-468f-9872-5ab7fefa9aa7.png)


## <br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>RESULT:
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
