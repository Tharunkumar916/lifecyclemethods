# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.
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
Developed by: Tharun Kumar V
Registeration Number : 212224240173
*/
```
### activity_main.xml
```python
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
        android:textSize="24sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
### AndroidManifest.xml
```python
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@drawable/ic_launcher_foreground"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.MobileAppdemo"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```
### MainActivity.java
```python
package com.example.mobileappdemo;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(),"onCreate Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(),"onRestart Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(),"onStop Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(),"onDestroy Called",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## OUTPUT
<img width="1254" height="700" alt="Screenshot 2025-09-22 210938" src="https://github.com/user-attachments/assets/9c7b258e-bc52-45ce-b1a6-11e892c7506e" />
<img width="1256" height="701" alt="Screenshot 2025-09-22 211317" src="https://github.com/user-attachments/assets/13ef372c-9a36-426a-b237-a5491abe5f9d" />
<img width="1254" height="695" alt="Screenshot 2025-09-22 211351" src="https://github.com/user-attachments/assets/d5d43bd1-088a-470e-86c9-b9980ec9f398" />
<img width="1247" height="690" alt="Screenshot 2025-09-22 211422" src="https://github.com/user-attachments/assets/e1586c4f-aee4-480a-b0a7-d630b9a86743" />
<img width="1250" height="695" alt="Screenshot 2025-09-22 211457" src="https://github.com/user-attachments/assets/c13d3495-c147-460c-9459-df8cc33cf33c" />







## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
