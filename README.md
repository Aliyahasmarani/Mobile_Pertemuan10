# Mobile_Pertemuan10

# 1. MEMBUAT LAYOUT UNTUK HALAMAN UTAMA (activity_main.xml)

### Berikut Codenya

```
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical">

        <GridLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:rowCount="1"
            android:columnCount="2"
            android:alignmentMode="alignMargins"
            android:columnOrderPreserved="false">
            <!--Menu 1-->
            <androidx.cardview.widget.CardView
                android:id="@+id/hallo"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">
                    <ImageView
                        android:layout_width="50dp"
                        android:layout_height="40dp"
                        android:src="@drawable/hallo" />
                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Hallo" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <!--Menu 2-->
            <androidx.cardview.widget.CardView
                android:id="@+id/fibo"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">

                    <ImageView
                        android:layout_width="50dp"
                        android:layout_height="40dp"
                        android:src="@drawable/count"/>

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Fibonacci"/>
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <!--Menu3-->
            <androidx.cardview.widget.CardView
                android:id="@+id/scroll"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">

                    <ImageView
                        android:layout_width="60dp"
                        android:layout_height="40dp"
                        android:src="@drawable/poison"/>

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Sianida"/>
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <!-- Menu 4-->
            <androidx.cardview.widget.CardView
                android:id="@+id/twoactivity"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">
                    <ImageView
                        android:layout_width="50dp"
                        android:layout_height="40dp"
                        android:src="@drawable/message"/>

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Message"/>
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <!--Menu5-->
            <androidx.cardview.widget.CardView
                android:id="@+id/SetAlarm"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">
                    <ImageView
                        android:layout_width="50dp"
                        android:layout_height="40dp"
                        android:src="@drawable/jam"/>

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Alarm"/>
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <!--Menu 6-->
            <androidx.cardview.widget.CardView
                android:id="@+id/showmap"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_columnWeight="1"
                android:layout_rowWeight="1"
                android:elevation="5dp"
                app:cardCornerRadius="100dp"
                app:cardUseCompatPadding="true">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="vertical"
                    android:gravity="center_horizontal"
                    android:padding="10dp">
                    <ImageView
                        android:layout_width="50dp"
                        android:layout_height="40dp"
                        android:src="@drawable/map"/>

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Maps"/>
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </GridLayout>
    </LinearLayout>
</ScrollView>
```

![image](https://github.com/Aliyahasmarani/Mobile_Pertemuan10/assets/115197672/e4931d74-3482-41aa-a2da-e1c593d4b952)

Saya menggunakan Icon external yang saya tambahkan pada `Drawable`. lalu saya panggil di dalam layout tersebut.

# 2. LALU, ADA TAMBAHAN DAN PERUBAHAN SEDIKIT PADA JAVANYA (MainActivity.java)

### Berikut Codenya

```
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;
import androidx.cardview.widget.CardView;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.provider.AlarmClock;
import android.view.View;

import com.google.android.material.button.MaterialButton;

public class MainActivity extends AppCompatActivity{


    private CardView btnSecond;
    private CardView btnFirst;
    private CardView btnHallo;
    private CardView btnFibo;
    private CardView btnAlarm;
    private CardView btnMaps;
    private CardView btnScroll;

    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        btnSecond = findViewById(R.id.twoactivity);
        btnFirst = findViewById(R.id.twoactivity);
        btnHallo = findViewById(R.id.hallo);
        btnFibo = findViewById(R.id.fibo);
        btnScroll = findViewById(R.id.scroll);
        btnAlarm = findViewById(R.id.SetAlarm);
        btnMaps = findViewById(R.id.showmap);

        setToolbar();
        setIntent();
    }

    private void setToolbar() {
        if (getSupportActionBar() != null) {
            getSupportActionBar().setTitle("USER");
            getSupportActionBar().setSubtitle("Projek Gabungan");
        }
    }

    private void setIntent() {
        btnSecond.setOnClickListener(view -> {
            Intent intent = new Intent(this, SecondActivity.class);
            startActivity(intent);
            finish();
        });

        btnFirst.setOnClickListener(view -> {
            Intent intent = new Intent (this, FirstActivity.class);
            startActivity(intent);
        });

        btnHallo.setOnClickListener(view -> {
            Intent intent = new Intent (this, HalloActivity.class);
            startActivity(intent);
        });

        btnFibo.setOnClickListener(view -> {
            Intent intent = new Intent (this, Fibonacci.class);
            startActivity(intent);
        });

        btnScroll.setOnClickListener(view -> {
            Intent intent = new Intent (this, ScrollSianida.class);
            startActivity(intent);
        });

        btnAlarm.setOnClickListener(view -> {
            Intent intent = new Intent (AlarmClock.ACTION_SHOW_ALARMS);
            startActivity(intent);
        });

        btnMaps.setOnClickListener(view -> {
            Uri geoLocation = null;
            Intent intent = new Intent(Intent.ACTION_VIEW);
            intent.setData(geoLocation);
            if (intent.resolveActivity(getPackageManager()) != null) {
                startActivity(intent);
            }
        });
    }


}
```

![image](https://github.com/Aliyahasmarani/Mobile_Pertemuan10/assets/115197672/ad398b7b-79b4-44d4-a015-68681a1c8dc5)


https://github.com/Aliyahasmarani/Mobile_Pertemuan10/assets/115197672/27197ba4-0031-4c7e-baa1-24961c522eb5



